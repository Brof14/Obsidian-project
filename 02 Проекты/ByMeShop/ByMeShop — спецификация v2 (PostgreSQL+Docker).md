
title: "ByMeShop — спецификация v2 (PostgreSQL+Docker)"
category: "Проекты/ByMeShop"
tags: [project, telegram-bot, aiogram, postgresql, docker, spec]
created: 2026-06-06
links: [[ByMeShop — обзор проекта]], [[ByMeShop — спецификация v1 (SQLite)]], [[Полезные команды Docker]]


# 🛒 ByMeShop — production-спецификация (v2, PostgreSQL + Docker)

> Расширенная версия спецификации: переход с SQLite-монолита ([[ByMeShop — спецификация v1 (SQLite)]]) на полноценный production-проект с PostgreSQL, Docker Compose и тремя платёжными методами.

## Роль и цель

Полностью сгенерировать production-ready проект Telegram-магазина цифровых товаров «ByMeShop»: готовый коммерческий магазин, собираемый в Docker, загружаемый на VPS и запускаемый без изменения кода.

## Стек

Python 3.12, aiogram 3.x, PostgreSQL, SQLAlchemy 2.0 Async, asyncpg, aiohttp, Pydantic Settings, Docker, Docker Compose, CryptoBot API, ЮKassa API, Telegram Stars, structlog.

## Архитектура

Без Enterprise Architecture / DDD / Repository Pattern / Clean Architecture — проект должен быть понятен одному разработчику.

```
bymeshop/
app/
├── handlers/
│   ├── games.py
│   ├── telegram_section.py
│   ├── services_section.py
│   ├── admin.py
│   └── payments.py
├── services/
│   ├── orders.py
│   ├── products.py
│   ├── payments.py
│   ├── reservations.py
│   └── statistics.py
├── keyboards/
│   └── keyboards.py
├── states/
│   └── states.py
├── database/
│   ├── models.py
│   ├── database.py
│   └── init_db.py
├── config.py
├── logger.py
└── main.py
Dockerfile
docker-compose.yml
.env.example
requirements.txt
README.md
backup.sh
```

## База данных

Модели: `users`, `orders`, `payments`, `items`, `reservations`, `broadcasts`, `settings`, `admins`. Полная реализация через SQLAlchemy, автосоздание таблиц.

## Функционал

Все разделы (Игры/Standoff 2, Brawl Stars, PUBG Mobile, Free Fire, Roblox / Телеграм / Сервисы → Steam) — логика идентична [[ByMeShop — спецификация v1 (SQLite)]], но БД переходит на PostgreSQL.

## Платежи

Одновременная реализация трёх методов: **ЮKassa**, **CryptoBot**, **Telegram Stars**. Для каждого: создание платежа, получение статуса, проверка оплаты, обновление заказа/платежа.

После оплаты: статус заказа → `PAID`, уведомление клиенту и админу (для Standoff Gold — со скриншотом скина).

## Админка (`/admin`)

Разделы: 📊 Статистика, 📦 Товары (➕ Добавить / ✏️ Изменить / 🗑 Удалить), 📢 Рассылка, 💰 Касса, 📈 Продажи, 👤 Пользователи, ⚙ Настройки.

**Рассылка** поддерживает текст, фото, видео, документ, инлайн-кнопки — по всем пользователям из БД.

## UI

Линии-разделители, эмодзи, важные данные (UID/Email/Логины/ID заказов/Суммы) в `<code>`, максимум `edit_text()` вместо новых сообщений, обязательные кнопки 🔙 Назад / ❌ Отмена.

## Безопасность

Rate Limit, FSM-защита, проверка прав администратора, проверка callback-данных, валидация пользовательского ввода, логирование ошибок.

## Docker

Полный `Dockerfile`, `docker-compose.yml`, контейнер PostgreSQL, volumes, `restart: always`, `.env`. Команды Docker — см. [[Полезные команды Docker]].

## Backup

`backup.sh` — резервное копирование PostgreSQL.

## README

Полная инструкция: установка, настройка `.env`, настройка ЮKassa/CryptoBot/Telegram Stars, запуск Docker, обновление, бэкапы, перенос на новый VPS.

## Формат вывода

Для каждого файла — заголовок `### FILE: путь_к_файлу` с полным кодом. После последнего файла — итоговая структура директорий и команда запуска:

```bash
docker compose up -d --build
```

## Критическое требование к генерации

Не выводить проект кусками — собрать полный набор файлов, без сокращений и пропущенных файлов. Финальный архив: `ByMeShop.zip` со всем исходным кодом, `Dockerfile`, `docker-compose.yml`, `.env.example`, `README.md`, `backup.sh`, `requirements.txt`.

> Реальные значения `.env` (токен бота, пароль БД, ключи ЮKassa и CryptoBot), найденные в исходных заметках, перенесены в [[Секреты — требуют внимания]].

---
**Связанные заметки:** [[ByMeShop — обзор проекта]], [[ByMeShop — спецификация v1 (SQLite)]], [[Полезные команды Docker]]

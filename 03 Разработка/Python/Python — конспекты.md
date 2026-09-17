
title: "Python — конспекты"
category: "Разработка/Python"
tags: [programming, python, notes]
created: 2026-06-06
links: [[Python]], [[metanit.com]]


# 🐍 Python — конспекты

> Личные заметки по ходу изучения на [[metanit.com]].

## Ввод / вывод

- `input()` — ввод данных от пользователя
- `print()` — вывод в консоль

## Ключевые слова Python

```python
False    await    else     import   pass
None     break    except   in       raise
True     class    finally  is       return
and      continue for      lambda   try
as       def      from     nonlocal while
assert   del      global   not      with
async    elif     if       or       yield
```

## Числовые системы счисления

| Система | Префикс | Пример |
|---|---|---|
| Двоичная | `0b` | `0b1010` = 10 |
| Восьмеричная | `0o` | `0o12` = 10 |
| Шестнадцатеричная | `0x` | `0xA` = 10 |

## Практика: приведение типов

```python
a = 5          # int()
b = 5.5        # float()
c = "Hello, World"  # str()
d = "9.5"      # str() -> float()
print(a + b + float(d))  # 20.0
```

![[Pasted image 20260606003903.png]]

## Практика: разбор числа на цифры по позициям

```python
number = int(input())
thousand = number // 1000          # находим 1-ю цифру
hundred = number % 1000 // 100     # находим 2-ю цифру
ten = number % 100 // 10           # находим 3-ю цифру
one = number % 10                  # находим 4-ю цифру

print(f'цифра в позиции тысяч равна {thousand}')
print(f'цифра в позиции сотен равна {hundred}')
print(f'цифра в позиции десятков равна {ten}')
print(f'цифра в позиции единиц равна {one}')
```

---
**Связанные заметки:** [[Python]], [[metanit.com]]

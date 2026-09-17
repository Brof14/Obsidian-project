(async function removeOnlyTrash() {
  // ИСКЛЮЧИТЕЛЬНО РАЗВЛЕКАТЕЛЬНЫЙ МУСОР И ИНФОШУМ:
  const trashTitles = [
    "A Week In The Life of MrBeast",
    "Асхаб Тамаев VS Филипп Марвин. Полный Бой.",
    "Гио Пика — как живет звезда шансон-рэпа: хит с Кравцем, невеста, родная деревня / Вписка",
    "GTA 6 (Grand Theft Auto 6) - Official Extended Gameplay",
    "LEVI ACKERMAN - AOT 4 「 AMV 」 Loving you is a losing game",
    "Гордон посетил санчасть в лагере для русских военнопленных",
    "Неадекваты, ночные бабочки и изменщики. Кто катается ночью в такси бизнес-класса",
    "Вопрос Ребром - Слава Бустер",
    "Что ВЫ почувствуете, если ВАМ ПЕРЕСАДЯТ ТЕЛО? — ТОПЛЕС",
    "Давидыч – русско-китайский автопром, развод из-за измены, тюрьма и ответ на хейт",
    "Nobody Can Handle Cillian Murphy's NONCHALANT Personality",
    "Амиран Сардаров — почему не уехал из России? Развод и рум тур в Москва-Сити / Вписка",
    "УЕХАЛ К ДЕДУ в НЬЮ-ЙОРК",
    "These Powerful Speeches Will Change Your Life | CR7 Motivation ( Cristiano Ronaldo )",
    "Внезапно на Земле остались 1 мужчина и 3 миллиарда женщин",
    "Почему Американцы такие необразованные?",
    "😱ТАМАЕВ ПОДАРИЛ ДОРОГОЙ ПОДАРОК РАВШАНУ😱| РЕАКЦИЯ ЛИТВИНА И СТИЛА НА БУГГАТИ !",
    "Блогеры VS Стримеры | ГЛАВНЫЙ ФУТБОЛЬНЫЙ МАТЧ ГОДА | КТО ЖЕ ПОБЕДИТ?",
    "Про женское тело и близость БЕЗ стыда. Посмотри это видео с мужчиной!",
    "Telegram конец? ФСБ возбудила дело против Дурова",
    "Парень Уничтожил Всех Онлифанок на Подкасте💣",
    "Вопрос Ребром - Матвей Сафонов",
    "Чем опасна зависимость от Порнографии?",
    "Я поняла, почему мужчины больше не бегают за женщинами. Теперь бегать будут женщины",
    "ПОЧЕМУ НЕ ТЫ?",
    "T2x2 СМОТРИТ: Я отправился в круиз только для взрослых с рейтингом «Х»",
    "I stayed in a 5* hotel in London",
    "Как американцы ЛЮБИЛИ Путина",
    "The Gentlemen cast REACT to shock deaths, season 3 and those Meghan Markle rumours",
    "Если бы мы переехали в Америку в 2025. Семейный подкаст",
    "Asking NY Billionaires How They Got Rich!",
    "Laziest Ways to Make Money with AI (For Beginners)"
  ];

  const cleanTitle = text => text.replace(/\s+/g, ' ').trim().toLowerCase();
  const removeSet = new Set(trashTitles.map(cleanTitle));

  const items = Array.from(document.querySelectorAll('ytd-playlist-video-renderer'));
  console.log(`🔍 Анализируем ${items.length} видео...`);

  let removedCount = 0;

  for (const item of items) {
    const titleElement = item.querySelector('#video-title');
    if (!titleElement) continue;

    const rawTitle = titleElement.innerText || titleElement.textContent;
    const formattedTitle = cleanTitle(rawTitle);

    if (removeSet.has(formattedTitle)) {
      console.log(`❌ УДАЛЯЕМ МУСОР: "${rawTitle.trim()}"`);

      const menuButton = item.querySelector('button[aria-label="Действия над видео"]') ||
                         item.querySelector('button[aria-label="Action menu"]') ||
                         item.querySelector('ytd-menu-renderer button');

      if (menuButton) {
        menuButton.click();
        await new Promise(r => setTimeout(r, 400));

        const menuItems = Array.from(document.querySelectorAll('ytd-menu-service-item-renderer, tp-yt-paper-item'));
        const deleteButton = menuItems.find(el => 
          el.innerText.includes('Удалить из') || 
          el.innerText.includes('Remove from')
        );

        if (deleteButton) {
          deleteButton.click();
          removedCount++;
          await new Promise(r => setTimeout(r, 800));
        } else {
          document.body.click();
        }
      }
    }
  }

  console.log(`\n🎉 Готово! Безопасно удалено мусорных роликов: ${removedCount}. Полезные видео по IT, Английскому, Алгоритмам и Науке оставлены!`);
})();
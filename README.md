<div align="center">
💅 Beauty Bot for Tatyana
Telegram-бот для онлайн-записи к мастеру красоты
Show Image
Show Image
Show Image
Show Image

Клиент выбирает дату через интерактивный календарь, оставляет имя и телефон — мастер получает готовую запись. Без сторонних сервисов, всё в Telegram.

</div>

📸 Скриншоты
Главное менюВыбор датыПодтверждениеShow ImageShow ImageShow Image

⚡ Возможности
👤 Для клиента
ФункцияОписание📅 ЗаписьИнтерактивный календарь — текущий и следующий месяц✅ ВалидацияПроверка телефона по коду страны и количеству цифр🔔 НапоминаниеАвтоматически за 24 часа до визита👁 УправлениеПросмотр и отмена своей записи💰 ПрайсАктуальные цены прямо в боте🖼 ПортфолиоГалерея работ мастера
🔧 Для мастера (панель администратора)

Добавление слотов по диапазону и шагу — например 10:00–18:00 каждые 30 или 60 мин
Удаление слотов и закрытие дня одной кнопкой
Расписание на любую дату

🛡 Надёжность

Защита от двойной записи на одно время
Автоматическое освобождение «зависших» броней (pending > 15 мин)
Восстановление всех напоминаний после перезапуска бота
Логирование ошибок в отдельный Telegram-канал


🗂 Стек
КомпонентТехнологияЯзыкPython 3.10+Telegram APIaiogram 3.x (FSM, inline-кнопки)База данныхSQLite через aiosqlite (асинхронно)Фоновые задачиAPScheduler — AsyncIOSchedulerКонфигpython-dotenv (.env)TimezoneEurope/Moscow

🚀 Быстрый старт
1. Клонировать репозиторий
bashgit clone https://github.com/AnonPit0404/beauty-bot.git
cd beauty-bot
2. Создать виртуальное окружение
bashpython -m venv venv
source venv/bin/activate        # macOS / Linux
# venv\Scripts\activate         # Windows
3. Установить зависимости
bashpip install -r requirements.txt
4. Настроить .env
envBOT_TOKEN=your_bot_token_here
ADMIN_ID=your_telegram_user_id
LOG_CHANNEL_ID=your_log_channel_id

Токен получить у @BotFather. Свой ADMIN_ID — у @userinfobot.

5. Запустить
bashpython bot.py

📁 Структура проекта
beauty_bot/
├── bot.py              # Точка входа, запуск поллинга
├── config.py           # Загрузка переменных окружения
├── states.py           # FSM-состояния (aiogram)
├── database.py         # Работа с SQLite (aiosqlite)
├── keyboards.py        # Inline-кнопки, календарь
├── handlers/
│   ├── client.py       # Логика для клиента
│   └── admin.py        # Панель мастера
└── utils/
    └── scheduler.py    # APScheduler, напоминания

🗺 Roadmap

 Запись через интерактивный календарь
 Валидация телефона
 Напоминания за 24 часа
 Панель администратора
 Защита от двойной записи
 Деплой на VPS
 Статистика для мастера
 Поддержка нескольких мастеров


👤 Автор
Антон Иванчиков — Junior QA Engineer
Show Image
Show Image

<div align="center">
<sub>Сделано с ☕ и aiogram 3</sub>
</div>

# MAI-Schedule
Бот для телеграмма, показывающий расписание, оповещающий о следующих парах и вообще прикольная утилита для настоящего маёвца!

# V 2.5
- Переписан весь функционал бота
- За основу GUI взята схема murych https://github.com/sergey27564/schedulemai/issues/3
- Функционал разбит на 3 отдельных модуля:
    * db_manage.py - работа с бд
    * dates.py - разбота с датой и временем
    * bot.py - основной функционал бота, который реализуется посредством использования модулей db_manage.py и dates.py
- Теперь расписание не парсится каждый раз при запросе пользователя, а запрашивается из таблицы бд
- Также была добавлена лицензия, после того как я узнал, что мое имя, наглым образом, не показывается в именах разработчиков бота
- Все написано соблюдая стандарты PEP8

# TODO
- Уведомления
- Объявления для пользователей

# INFO
- Для работы необходимо создать файл secret_settings.py в той же
директории, в которой находится данный файл. В secret_settings.py
необходимо добавить 2 строчки:
    * TOKEN = Ваш токен
    * DB_NAME = Имя вашей базы данных, например bot.sqlite3
- Также, в файле config.py, необходимо установить значения START_YEAR, START_MONTH и
START_DAY. Эти значения нужно будет изменять при начале нового семестра.

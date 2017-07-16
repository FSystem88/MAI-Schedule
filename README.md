# MAI-Schedule
Бот для телеграмма, показывающий расписание, оповещающий о следующих парах и вообще прикольная утилита для настоящего маёвца!

# V 2.2
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
- Написать декоратор в bd_manage.py, который бы обеспечивал работу с курсором
- Закомментировать код
- Уведомления
- Объявления для пользователей

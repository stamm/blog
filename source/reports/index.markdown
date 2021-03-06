---
layout: page
title: "Доклады и мастер-классы"
date: 2014-01-31 16:14
comments: true
sharing: true
footer: true
---

{% render_partial reports/toc.markdown %}

# <a id="reports"></a>Доклады

## <a id="librarian"></a>Повторяемость для котиков: библиотекарь и книжная полка

Поговорим о проблемах командного изменения конфигурации, а также управления версиями и зависимостями сторонних библиотек
(в терминах Chef — кукбуков):

* где хранить сторонние кукбуки;
* как сделать, чтобы у всех инженеров был одинаковый «срез» конфигурации;
* как обновлять свои и сторонние кукбуки с учетом их зависимостей.

В докладе описаны два современных инструмента для решения этих проблем: librarian-chef и Berkshelf. Мы сравним их,
разберем сильные и слабые стороны, особенности интеграции с системой создания окружений Vagrant. Также посмотрим на
практики использования этих инструментов, выработанные в компании «Экспресс 42».

Доклад прочитан 25 января 2014 года на [DevOps митапе в Яндексе](http://tech.yandex.ru/events/yagosti/devops/),
[слайды](http://www.slideshare.net/evtuhovich/2014-01-yandex) и
[видео](http://tech.yandex.ru/events/yagosti/devops/talks/1597/).

## <a id="continuousdelivery"></a>Continuous Delivery. Как перестать релизиться и начать жить

Если

* каждый ваш релиз — это головная боль и бессонная ночь;
* системные администраторы показывают пальцем на программистов, а программисты на сисадминов, но все равно ничего не работает;
* поменять что-то на боевых серверах так, чтобы ничего не упало, практически невозможно.

Тогда этот доклад — для вас.

Этот доклад расскажет про:

* основные инженерные практики, которые позволяют сделать процесс внесения изменений в уже существующий проект более дешевым и быстрым;
* интеграцию каждого комита сразу после попадания в систему контроля версий;
* алгоритм запуска циклов обратной связи на самых ранних стадиях, когда вносить изменения и править ошибки дешевле всего;
* описание процесса, как сделать время попаданий изменений в «бой» минимальным.

Весь доклад подкреплен реальными историями из личного опыта автора.

Опыт консультирования в компании „Экспресс 42“ показывает, что использование современных подходов в разработке
IT-проектов — достаточно редкая практика. Зачастую многие программные инструменты используются без понимания, зачем это
нужно, просто из любопытства или шумихи вокруг них. Данный доклад призван это исправить.

Продолжительность доклада 45-60 минут. Доклад читался на [конференции SECON в Пензе](http://2013.secon.ru/) в 2013 году,
[слайды можно найти здесь](http://www.slideshare.net/evtuhovich/continuousdelivery).

## <a id="rmongorb"></a>Нетрадиционное использование Ruby и PostgreSQL
Слегка несерьезный доклад о том, как использовать язык Ruby не для разработки Web-приложений. Доклад состоит
из трех частей.

Первая часть рассказывает о том, как можно использовать Ruby внутри редактора Vim. Рассказывается о возможностях
интеграции и ее ограничениях, а также рассказывается о том, как рисовать ковер Серпинского.

Вторая часть рассказывает о том, как можно использовать нестандартные типы PostgreSQL hstore и array внутри Ruby
приложения с использованием библиотеки ActiveRecord.

Третья часть доклада рассказывает и показывает, как, используя язык ruby (а именно pl/ruby), yaml как формат хранения данных и
PostgreSQL, создать rmongo.rb – NoSQL базу данных с интерфейсом, практически полностью идентичным MongoDB.

Продолжительность доклада 25 минут. Доклад читался на конференции Railsclub'Ulsk в Ульяновске в 2012 году, слайды лежат
[здесь](http://www.slideshare.net/evtuhovich/ruby-postgresql).

## <a id="grpn"></a>Как мы делали Групон
В докладе рассказывается о том, как сотрудники EvilMartians делали сайт groupon.ru. Рассказывается об
архитектуре проекта, о его внутреннем устройстве, о типичных проблемах, с которыми пришлось столкнуться. Также 
освещаются вопросы организации командной работы, управления конфигурацией, выкатки. Обзорно рассказывается о
Open Source проектах, которые были выпущены в процессе создания http://groupon.ru.

В архитектуре проекта описывается внутреннее устройство сайта groupon.ru, используемые программные продукты (nginx,
debian, ruby, rails, postgresql, memcached) и особенности их настройки.

В типичных проблемах я расскажу 3-5 интересных случая из разработки групона: какая проблема возникла и как мы ее решали.

Также я расскажу о том, как устроена команда, как происходит процесс управления разработкой, как мы тестируем, релизимся
и какие инструменты для этого используем.

В части про управление конфигурацией я расскажу о том, с какими проблемами администрирования мы сталкивались, почему и
как мы переехали на систему управления конфигурацией (opscode chef). Также я расскажу о том, как происходят выкатки с
помощью capistrano.

В последней части я расскажу о библиотеках, которые была написаны и отданы в OpenSource в процессе
создания групона. Это zendesk, gon, cupid, visibility.js, role.

Доклад читался 2 раза — на конференции [Toster](http://toster.ru/conferences/10-02-2012-ruby/results) в Москве в 2012
году и на конференции [CodeFest](http://www.youtube.com/watch?v=s5HcEAR6THQ) в Новосибирске в 2012 году, слегка
измененным для аудитории, незнакомой с языком Ruby.

## <a id="vimordie"></a>Vim Or Die

Доклад об одном из самых мощных современных текстовых редакторах — Vim. В докладе расскрываются самые важные базовые
возможности Vim, а также описываются популярные плагины для Vim, которые делают работу с этим редактором еще более
эффективной.

Доклад читался один раз в 2010 году на конференции [Railsclub](http://railsclub.ru), вызвал бурю эмоций и новую волну
священных войн. [Слайды можно посмотреть на Slideshare](http://www.slideshare.net/evtuhovich/vim-or-die), а
видео доклада лежит [здесь](http://univertv.ru/video/informatika/programmirovanie/ruby_on_rails_moscow/vim_or_die/).

# <a id="master-class"></a>Мастер-классы
## <a id="pg"></a>Устройство и оптимизация Postgresql
Мастер класс рассчитан на разработчиков и администраторов БД любого уровня, материал будет подобран под конкретную
аудиторию. В мастер-классе освещается внутреннее устройство PostgreSQL (с упором на версию 9.2), рассказывается о
типичных проблемах, с которыми приходится встречаться при эксплуатации этой БД, а также о путях их решения.

Материал читался на конференции CodeFest, частями читался в рамках мастер-класса [Brainwashing](http://brainwashing.pro/),
а также у клиентов компании «[Экспресс 42](http://express42.com/)».

Приблизительный план мастер-класса следующий:

1. Аппаратное обеспечение
   1. RAID
   2. Write cache
   3. Настройка дисков
   4. Настройки ОС
1. Структура папок
1. Память
   1. Структура использования памяти
1. Настройки PostgreSQL
   1. Логирование
   1. Vacuum
   1. Checkpoint
5. Транзакции
   1. ACID
   2. Уровни изоляции
   1. Лог транзакций
   2. Блокировки
   3. Deadlock
1. Обслуживание
   1. MVCC
   1. Vacuum
   1. Логирование запросов
1. Индексы
    1. Деревья
    2. Селективность индекса
    3. Частичные индексы
    4. Функциональные индексы
1. Оптимизация запросов
    1. Статистика
    2. Планировщик запросов
    3. Денормализация данных
       1. Счетчики
       2. Поиск
1. Статистика использования таблиц и индексов
1. Мониторинг
1. PgBouncer и pgPool
1. Репликация
7. Шардинг
    1. Архивирование таблиц
    2. Вертикальный шардинг
    3. Горизонтальный шардинг
1. Решение типичных проблем, возникающих с PostgreSQL

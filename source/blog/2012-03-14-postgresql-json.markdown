---
layout: post
title: Поддержка JSON в PostgreSql 9.2
date: 2012-03-14 23:52
comments: true
categories:
- json
- PostgreSQL
---

В третьем квартале 2012 должна выйти версия [PostgreSQL 9.2](http://www.postgresql.org/developer/roadmap/), в которой
добавят много интересных возможностей. Среди них — базовая поддержка так полюбившегося всем web-разработчикам формата
JSON. На данном этапе появится только возможность [проверять JSON на валидность](http://www.postgresql.org/docs/devel/static/datatype-json.html),
но судя по списку рассылки, к версии 9.3 будет добавлена возможность строить индексы на JSON объектах подобно тому, как
это [можно сделать на hstore](/blog/2012/01/23/hstore/). Конечно, JSON объекты гораздо сложнее hstore, и как именно и в
каком объеме будет реализована поддержка индексов в JSON — пока не ясно.

Postgres развивается, а это не может не радовать.

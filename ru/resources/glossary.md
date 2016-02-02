---
### TRANSLATION INSTRUCTIONS FOR THIS SECTION:
### TRANSLATE THE VALUE OF THE title ATTRIBUTE AND UPDATE THE VALUE OF THE lang ATTRIBUTE.
### DO NOT CHANGE ANY OTHER TEXT.
layout: page
title: Глоссарий по Express
menu: resources
lang: ru
### END HEADER BLOCK - BEGIN GENERAL TRANSLATION
---

# Глоссарий

<div class="doc-box doc-warn">На данный момент это рабочая черновая версия</div>

### application (приложение)

В общем смысле, одна или несколько программ, предназначенных для выполнения операций с определенной целью.  В контексте Express - программа, использующая API Express, запущенный на платформе Node.js.  Также называется [объектом приложения](/{{ page.lang }}/api.html#express).

### API

Интерфейс программирования приложений.  Рекомендуется расшифровывать данную аббревиатуру при первом упоминании.

### Express

Быстрый, гибкий, минималистичный веб-фреймворк для приложений Node.js.  В целом, название "Express" является более предпочтительным, чем"Express.js", хотя последнее тоже допускается.

### libuv

Библиотека мультиплатформной поддержки, ориентированная на асинхронный ввод/вывод, в основном разработанный для использования Node.js.

### middleware (промежуточные обработчики)

Функция, вызываемая уровнем маршрутизации Express перед обработчиком финального запроса, то есть, находящаяся между необработанным запросом и окончательным заданным маршрутом.  Вот некоторые выдержки из терминологии, связанной с промежуточными обработчиками:

  * `var foo = require('middleware')` называется *затребованием* или *использованием* модуля Node.js. Затем оператор `var mw = foo()`, как правило, возвращает промежуточный обработчик.
  * `app.use(mw)` называется *добавлением промежуточного обработчика в глобальный стек обработки*.
  * `app.get('/foo', mw, function (req, res) { ... })` называется *добавлением промежуточного обработчика в стек обработки "GET /foo"*.

### Node.js

Платформа программного обеспечения, используемая для разработки масштабируемых сетевых приложений. Node.js использует JavaScript в качестве языка создания сценариев и обеспечивает высокую пропускную способность благодаря неблокирующему вводу/выводу и однопотоковому циклу событий.  См. [nodejs.org](http://nodejs.org/). **Особенность употребления термина**: При первом упоминании - "Node.js", в дальнейшем - "Node".

### open-source, open source (открытый исходный код, с открытым исходным кодом)

В английском языке прилагательное open-source пишется через дефис; например: "This is open-source software" ("Это программное обеспечение с открытым исходным кодом"). См. статью [Открытое программное обеспечение](http://en.wikipedia.org/wiki/Open-source_software) в Википедии. Примечание: Хотя широко распространено употребление данного термина без дефиса, мы следуем стандартным правилам английского языка, согласно которым составные прилагательные пишутся через дефис.

### request (запрос)

Запрос HTTP.  Клиент передает на сервер сообщение-запрос по протоколу HTTP, а сервер возвращает ответ.  В запросе должен использоваться один из нескольких [методов запроса](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol#Request_methods), например, GET, POST и т.д.

### response (ответ)

Ответ HTTP. Сервер возвращает клиенту сообщение-ответ по протоколу HTTP. Ответ содержит информацию о состоянии выполнения запроса, а также в теле сообщения может быть включено запрашиваемое содержимое.

### route (маршрут)

Часть URL, идентифицирующая ресурс.  Например, в `http://foo.com/products/id`, "/products/id" является маршрутом.

### router (маршрутизатор)

См. раздел [маршрутизатор](/{{ page.lang }}/4x/api.html#router) в справочнике API.
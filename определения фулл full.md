# 1 лек
## OSI
**Open Systems Interconnection model** (**OSI model**)
[reference model](https://en.wikipedia.org/wiki/Reference_model "Reference model") from the [International Organization for Standardization](https://en.wikipedia.org/wiki/International_Organization_for_Standardization "International Organization for Standardization") (ISO) that "provides a common basis for the coordination of standards development for the purpose of systems interconnection."[source](https://en.wikipedia.org/wiki/OSI_model)
## уровни протоколов?
## HTTP
HyperText Transfer Protocol
протокол прикладного уровня, на котором упрощенно говоря общаются браузер и веб сервер. это протокол предметной области -- он знает что такое web, какие атрибуты(свойства) есть у запросов и у ответов (лекция)
**HTTP** — это [протокол](https://developer.mozilla.org/ru/docs/Glossary/Protocol), позволяющий получать различные ресурсы, например HTML-документы.
Можно передавать также изображения и т п!

факты:
https = http завернутый в tls чтобы шифровать
HTTP является протоколом прикладного уровня, который чаще всего использует возможности другого протокола - [TCP](https://developer.mozilla.org/ru/docs/Glossary/TCP) (или [TLS](https://developer.mozilla.org/ru/docs/Glossary/TLS) - защищённый TCP) - для пересылки своих сообщений, однако любой другой надёжный транспортный протокол теоретически может быть использован для доставки таких сообщений.
## TCP **Transmission Control Protocol**
**TCP (Протокол Управления Передачей)** - важный [протокол](https://developer.mozilla.org/ru/docs/Glossary/Protocol) сети интернет, который позволяет двум хостам создать соединение и обмениваться потоками данных. TCP гарантирует доставку данных и пакетов в том же порядке, в котором они были отправлены.
лекция:
TCP -- протокол с помощью которого сетевые интерфейсы взаимодействуют между собой устанавливая надежное (reliable-)соединение
это делается трехвазным рукопожатием во время установки соединения -- небыстрая тема
## UDP
(User Datagram Protocol) is a long standing [protocol](https://developer.mozilla.org/en-US/docs/Glossary/Protocol) used together with [IP](https://developer.mozilla.org/en-US/docs/Glossary/IPv6) for sending data when transmission speed and efficiency matter more than security and reliability.
С UDP компьютерные приложения могут посылать сообщения (в данном случае называемые [датаграммами](https://ru.wikipedia.org/wiki/%D0%94%D0%B5%D0%B9%D1%82%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0 "Дейтаграмма")) другим [хостам](https://ru.wikipedia.org/wiki/%D0%A5%D0%BE%D1%81%D1%82 "Хост") по [IP-сети](https://ru.wikipedia.org/wiki/IP "IP") без необходимости предварительного сообщения для установки специальных [каналов передачи](https://ru.wikipedia.org/wiki/%D0%9A%D0%B0%D0%BD%D0%B0%D0%BB_%D0%BF%D0%B5%D1%80%D0%B5%D0%B4%D0%B0%D1%87%D0%B8_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85 "Канал передачи данных") или путей данных.
UDP использует простую модель передачи, без явных «рукопожатий» для обеспечения надёжности, упорядочивания или целостности данных.
Датаграммы могут прийти не по порядку, дублироваться или вовсе исчезнуть без следа, но гарантируется, что если они придут, то в целостном состоянии.
## TLS
transport layer security — Протокол защиты транспортного уровня
как и его предшественник [SSL](https://ru.wikipedia.org/wiki/SSL "SSL") ([англ.](https://ru.wikipedia.org/wiki/%D0%90%D0%BD%D0%B3%D0%BB%D0%B8%D0%B9%D1%81%D0%BA%D0%B8%D0%B9_%D1%8F%D0%B7%D1%8B%D0%BA "Английский язык") secure sockets layer — слой защищённых сокетов), — [криптографические протоколы](https://ru.wikipedia.org/wiki/%D0%9A%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B3%D1%80%D0%B0%D1%84%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%BF%D1%80%D0%BE%D1%82%D0%BE%D0%BA%D0%BE%D0%BB "Криптографический протокол"), обеспечивающие защищённую передачу данных между узлами в сети [Интернет](https://ru.wikipedia.org/wiki/%D0%98%D0%BD%D1%82%D0%B5%D1%80%D0%BD%D0%B5%D1%82 "Интернет")[[2]](https://ru.wikipedia.org/wiki/TLS#cite_note-2).
Протоколы SSL и TLS

|Протокол|Дата публикации|Состояние|
|---|---|---|
|SSL 1.0|не публиковался|не публиковался|
|SSL 2.0|1995|Признан устаревшим в 2011 году ([RFC 6176](https://tools.ietf.org/html/rfc6176))|
|SSL 3.0|1996|Признан устаревшим в 2015 году ([RFC 7568](https://tools.ietf.org/html/rfc7568))|
|TLS 1.0|1999|Признан устаревшим в 2020 году[[6]](https://ru.wikipedia.org/wiki/TLS#cite_note-:2-6)|
|TLS 1.1|2006|Признан устаревшим в 2020 году[[6]](https://ru.wikipedia.org/wiki/TLS#cite_note-:2-6)|
|TLS 1.2|2008||
|TLS 1.3|2018||

## user-agent
-- это любой инструмент или устройство, действующие от лица пользователя. Эту задачу преимущественно выполняет веб-браузер.
## Прокси
Между веб-браузером и сервером находятся большое количество сетевых узлов, передающих HTTP сообщения. Из-за слоистой структуры большинство из них оперируют также на транспортном сетевом или физическом уровнях, становясь прозрачным на HTTP слое и потенциально снижая производительность. Эти операции на уровне приложений называются **прокси**. Они могут быть прозрачными или нет, (изменяющие запросы не пройдут через них), и способны исполнять множество функций:
- caching (кеш может быть публичным или приватными, как кеш браузера)
- фильтрация (как сканирование антивируса, родительский контроль, …)
- выравнивание нагрузки (позволить нескольким серверам обслуживать разные запросы)
- аутентификация (контролировать доступом к разным ресурсам)
- протоколирование (разрешение на хранение истории операций)


## http-запрос:
![[Pasted image 20240310143911.png]]
![[Pasted image 20240206191709.png]]
- HTTP-[метод](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods), обычно глагол подобно [`GET`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/GET), [`POST`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/POST) или существительное, как [`OPTIONS`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/OPTIONS) или [`HEAD`](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods/HEAD), определяющее операцию, которую клиент хочет выполнить
- Путь к ресурсу
- Версию HTTP-протокола.
## заголовки (optional)
**заголовки HTTP** позволяют клиенту и серверу отправлять дополнительную информацию с HTTP запросом или ответом. В HTTP-заголовке содержится не чувствительное к регистру название, а затем после (`:`) непосредственно значение. [Пробелы](https://developer.mozilla.org/ru/docs/Glossary/Whitespace) перед значением игнорируются.
Заголовки могут быть сгруппированы по следующим контекстам:

- [Основные заголовки](https://developer.mozilla.org/ru/docs/Glossary/General_header) применяется как к запросам, так и к ответам, но не имеет отношения к данным, передаваемым в теле.
- Заголовки запроса содержит больше информации о ресурсе, который нужно получить, или о клиенте, запрашивающем ресурс.
- [Заголовки ответа (en-US)](https://developer.mozilla.org/en-US/docs/Glossary/Response_header "Currently only available in English (US)") содержат дополнительную информацию об ответе, например его местонахождение, или о сервере, предоставившем его.
- [Заголовки сущности](https://developer.mozilla.org/ru/docs/Glossary/Entity_header) содержат информацию о теле ресурса, например его [длину содержимого](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers/Content-Length) или тип [MIME (en-US)](https://developer.mozilla.org/en-US/docs/Web/SVG/Content_type "Currently only available in English (US)").
Заголовки также могут быть сгруппированы согласно тому, как [прокси (proxies)](https://developer.mozilla.org/ru/docs/Glossary/Proxy_server) обрабатывают их:

- [`Connection`](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers/Connection)
- [`Keep-Alive` (en-US)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Keep-Alive "Currently only available in English (US)")
- [`Proxy-Authenticate` (en-US)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Proxy-Authenticate "Currently only available in English (US)")
- [`Proxy-Authorization` (en-US)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Proxy-Authorization "Currently only available in English (US)")
- [`TE` (en-US)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/TE "Currently only available in English (US)")
- [`Trailer` (en-US)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Trailer "Currently only available in English (US)")
- [`Transfer-Encoding` (en-US)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Transfer-Encoding "Currently only available in English (US)")
- [`Upgrade` (en-US)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Upgrade "Currently only available in English (US)").
## параметры запроса
параметры у запроса (своего рода) бывают 2х видов:
1. get-параметры -- которые содержатся в get строке -- используются в основном для гет запросов -- могут быть доступны и видны промежуточным прокси-серверам, попадают в логи
2. которые находятся в самом запросе лол

семантика методов
## ответ
![[Pasted image 20240310143933.png]]
## статусный код
Код состояния ответа HTTP показывает, был ли успешно выполнен определённый [HTTP](https://developer.mozilla.org/ru/docs/Web/HTTP) запрос. Ответы сгруппированы в 5 классов:
1. [Информационные ответы](https://developer.mozilla.org/ru/docs/Web/HTTP/Status#%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D0%B5_%D0%BE%D1%82%D0%B2%D0%B5%D1%82%D1%8B) (`100` – `199`)
2. [Успешные ответы](https://developer.mozilla.org/ru/docs/Web/HTTP/Status#%D1%83%D1%81%D0%BF%D0%B5%D1%88%D0%BD%D1%8B%D0%B5_%D0%BE%D1%82%D0%B2%D0%B5%D1%82%D1%8B) (`200` – `299`)
3. [Сообщения о перенаправлении](https://developer.mozilla.org/ru/docs/Web/HTTP/Status#%D1%81%D0%BE%D0%BE%D0%B1%D1%89%D0%B5%D0%BD%D0%B8%D1%8F_%D0%BE_%D0%BF%D0%B5%D1%80%D0%B5%D0%BD%D0%B0%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B8) (`300` – `399`)
4. [Ошибки клиента](https://developer.mozilla.org/ru/docs/Web/HTTP/Status#%D0%BE%D1%88%D0%B8%D0%B1%D0%BA%D0%B8_%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D0%B0) (`400` – `499`)
5. [Ошибки сервера](https://developer.mozilla.org/ru/docs/Web/HTTP/Status#%D0%BE%D1%88%D0%B8%D0%B1%D0%BA%D0%B8_%D1%81%D0%B5%D1%80%D0%B2%D0%B5%D1%80%D0%B0) (`500` – `599`)
Коды состояния определены в [RFC 9110](https://httpwg.org/specs/rfc9110.html#overview.of.status.codes). Но по сути это просто семантика
[`200 OK`](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/200)
[`400 Bad Request`](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/400)
[`404 Not Found`](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/404)
[`408 Request Timeout`](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/408)
[`504 Gateway Timeout`](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/504)
[`500 Internal Server Error`](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/500)
[`502 Bad Gateway`](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/502)

## keep-alive
в 1.1 был придуман keep-alive концепция -- когда user-agent устанавливает соединение с сервером и может не разрывать его и уже в рамках этого соединения можно посылать много реквестов респонсов
кип-элайвы не бесконечны -- обычно 10ки-100ни секунд
## stateless в контексте http
понятно что, сказать про куки и сессии
## session
есть куки на сервере хранится мапа называем сессией

## URI
URI это в принципе концепция , объединение URL и URN
но какая то организация это регулирует
![[Pasted image 20240206164730.png]]
## URL
-- "унифицированный локатор ресурсов" , местоположение ресурсов в интернете
будем обращаться к базам данных и вместо foo будет mysql или jdbc 
может быть ssh
для http дефолтный порт это 80
https -- 443
fragment: после решетки -- определенный кусок на странице куда проскроллить
![[Pasted image 20240206181500.png]]

## сокет
конечная точка соединения
DNS
## ip адрес
**IP-адрес** (от англ. [Internet Protocol](https://ru.wikipedia.org/wiki/Internet_Protocol "Internet Protocol")) — уникальный числовой [идентификатор](https://ru.wikipedia.org/wiki/%D0%98%D0%B4%D0%B5%D0%BD%D1%82%D0%B8%D1%84%D0%B8%D0%BA%D0%B0%D1%82%D0%BE%D1%80 "Идентификатор") устройства в компьютерной [сети](https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BC%D0%BF%D1%8C%D1%8E%D1%82%D0%B5%D1%80%D0%BD%D0%B0%D1%8F_%D1%81%D0%B5%D1%82%D1%8C "Компьютерная сеть"), работающей по протоколу [IP](https://ru.wikipedia.org/wiki/IP "IP").

## докинуть про
OSI и tcp/ip
ssh
smtp
telnet
cache-control (общие слова)
доп:
файлик hosts
реверс-прокси
nginx как пример
# 2 лек
## HTML
HTML (Hypertext Markup Language) - это _язык разметки_, который используется для структурирования и отображения веб-страницы и её контента.
## структора html

```
<!doctype html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Моя тестовая страница</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="Моё тестовое изображение" />
  </body>
</html>
```
элемент [`<title>`](https://developer.mozilla.org/ru/docs/Web/HTML/Element/title). Этот элемент устанавливает заголовок для вашей страницы, который является названием, появляющимся на вкладке браузера загружаемой страницы, и используется для описания страницы, когда вы добавляете её в закладки/избранное.
## DOM
![[Pasted image 20240208214240.png|525]]
**Например**: стандарт DOM описывает, что метод `getElementsByTagName` в коде, указанном ниже, должен возвращать список всех элементов p в документе.
```
paragraphs = document.getElementsByTagName("P");
// paragraphs[0] это первый <p> элемент
// paragraphs[1] это второй <p> элемент и т.д.
alert(paragraphs[0].nodeName);
```
## элементы
Элемент - это часть веб-страницы. В XML и HTML элемент может содержать данные, фрагмент текста или изображения, или не содержать ничего. Обычный элемент включает в себя открывающий тэг с некоторыми атрибутами, текст и закрывающий тэг.
Элементы и тэги это _не_ одни и те же вещи. Тэги открывают или закрывают элементы в исходном коде, тогда как элементы являются частью [DOM](https://developer.mozilla.org/ru/docs/Glossary/DOM), объектной моделью документа для отображения страницы в [браузере](https://developer.mozilla.org/ru/docs/Glossary/Browser).

## блоковые элементы, структура
(блочные) -- по умолчанию занимает в **ширину** сколько может, а **высоту** сколько минимально нужно. 
![[Pasted image 20240208223235.png|550]]
**margin** -- внешний отступ
**border** -- граница
**padding** -- отступ контента от бордера
когда мы руками устанавливаем width/height, то по дефолту он устанавливается для контента
чтобы это поведение менять юзаем **box-sizing**
![[Pasted image 20240208224404.png]]
значения **margin-box** кажется не существует

## строковые элементы
![[Pasted image 20240208224558.png|425]]
к inline неприменимы верхние/нижние отступы и ширина
inline-block -- не разрывает строку, но можно указывать левые/правые отступы и т п

## строение элемента
![[Pasted image 20240310150458.png]]
Элементы также могут иметь **атрибуты**, которые выглядят так:
![[Pasted image 20240310150507.png]]
## атрибуты
Атрибуты содержат дополнительную информацию об элементе, которую вы не хотите показывать в фактическом контенте. 

Атрибут всегда должен иметь:

1. Пробел между ним и именем элемента (или предыдущим атрибутом, если элемент уже имеет один или несколько атрибутов).
2. Имя атрибута, за которым следует знак равенства.
3. Значение атрибута, заключённое с двух сторон в кавычки.
## - виды элементов 
Элементы можно разделить на:
- **inline**-элементы -- типа кусочек строки, могут даже начаться на одной строке и перенестись на другую строку. 
	Примеры (соответствующих тегов): p, div, main, header, section, article
- **блоковые** (блочные) -- по умолчанию занимает в **ширину** сколько может, а **высоту** сколько минимально нужно. 
Эти режимы отображения можно насильственно менять (см [[2 -- HTML + CSS#^displaySlide]])
по сути в html теги одного типа делают одно и тоже, разные названия передают семантику
ну только **div и span не обладают семантикой**, это простой блоковый и inline ~~элементы~~ определения элементов соответственно
## - теги
В [HTML](https://developer.mozilla.org/ru/docs/Glossary/HTML) теги используются для создания элементов. **Имя** HTML-элемента - это **имя** заключённое в угловые скобки, как например <p> для "абзаца". Обратите внимание, что концу **имени** предшествует символ косой черты (слеша), "</p>", и что в пустых элементах закрывающий тег не требуется и не допускается. Если атрибуты не указаны, то для них применяются значения по умолчанию.
## REM
"root-em"
размер шрифта в документе
величина размера
## CSS
## структура css-файла
![[Pasted image 20240208215331.png|525]]

## селектор
декларативный запрос к **DOM** (Document Object Model = дереву документа) "найди набор элементов из этого дерева"

## составные селекторы (механики)

- пробел =  "предок->потомок"
	note: потомок, а не сын
- больше = "родитель->ребенок"
![[Pasted image 20240208221926.png|129]]
- запятая=объединение путей, "или"
- двоеточие=псевдоклассы -- всякие штуки)) 
- псевдоклассы:
![[Pasted image 20240208222919.png|475]]
![[Pasted image 20240208223026.png|155]] ![[Pasted image 20240208223054.png|147]]
![[Pasted image 20240208234907.png|250]]
**Не путать!**
 "пэшка" с id="mike":
![[Pasted image 20240208222239.png]]
 id="mike" у которого есть предок "пэшка":
![[Pasted image 20240208222408.png]]
```
p : { } -- все теги <p>
* : { } -- ВСЕ элементы
#[идентефикатор] { } -- для 
<[тег] id="[идентефикатор]">...</>

предполагается что id уникальны

.[класс] { 
} -- для всех 
<[тег] class="[класс1 класс ...]">...</>

```

## position
![[Pasted image 20240208224916.png|475]]
речь идет про блоковые элементы
**relative** -- нарисовали как статик, а потом вырезали и подвинули (все размеры не меняются)
**absolute** -- забываем про контекст, отображаем от какой-то "точки отсчета", другие элементы про него не знают (не должны знать, забывают)
**точка отсчета**: дефолтно -- левый верхний угол, иначе -- идем вверх по дереву до первого элемента с **position: relative**
**fixed** -- абсолютно относительно левого верхнего угла браузера а не документа, например для уведомлений
## поплавки
![[Pasted image 20240208225821.png|475]]
## normalize.css
у браузера есть встроенные типа-css-ки которые говорят какие отступы делать на элементах по умолчанию
хотим ? верстку которая будет одинаково смотреться во всех бразерах в мире
есть два пути:
1. ресетнуть нахуй все
2. сделать нормалайз -- сбросить стили до нормального одинакового четкого значения во всех браузерах
#непонел 

допилить:
нормалайз
@media
# 3 лек
API
war
maven3
утилита mvn
архетип
артефакты
pom.xml
`scope:provided`

Servlet API, servlet
сессия
doXXX
tomcat
Catalina
# 4 лек
freemarker
шаблонизатор
как работает (пример из нашего проекта)
макросы
функции
аннотации
# 5+6 лек
MVC
схемки, примеры, описание реализации с 5 лекции
раутинг
домен
доменные сущности
сервис
контроллер
java reflection
схемки схемки схемки
соль в паролях
JDBC, что использовали
prepared statement
primary-ключ
индекс дерево поиска
# 7 лек
jquery
CDN
что используем из jquery
ajax
window
почему .prop("content")
так а зачем нужен ajax?
# 8 лек
SPRING
фреймворк
convention over configuration
spring initialiser
spring boot
spring web
JPA
Hibernate
ORM
аннотации 
@Repository
@Query
@Controller
@Component
@GetMapping
@ModelAttribute
@Valid
аннотации для валидации
BindingResult
@InitBinder
Spring bind-механика
@Autowired
IoC, DI
# лек 9
spring core
иногда можем и через properties аннотацией autowired ???
виды взаимосвязей объектов
практика
interceptor
про ленивость
#### реально не знал
что в html означает тег template

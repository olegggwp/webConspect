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
HTML
DOM
структура html-файла
- атрибуты
- директива link
- элементы
- виды элементов 
- теги
REM
CSS
структура css-файла
селектор
составные селекторы (механики)
псевдоклассы (тоже про составные селекторы)
блоковые элементы, структура
margin
border
padding
строковые элементы
position
поплавки
normalize.css
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

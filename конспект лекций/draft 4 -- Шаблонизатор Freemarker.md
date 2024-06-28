	шаболданизатор
**Apache FreeMarker** is a _template engine_: a Java library to generate text output (HTML web pages, e-mails, configuration files, source code, etc.) based on templates and changing data.
Templates are written in the FreeMarker Template Language (FTL), which is a simple, specialized language (not a full-blown programming language like PHP). Usually, a general-purpose programming language (like Java) is used to prepare the data (issue database queries, do business calculations). Then, Apache FreeMarker displays that prepared data using templates. In the template you are focusing on how to present the data, and outside the template you are focusing on what data to present.
[отсюда](https://freemarker.apache.org/index.html)

чтобы .ftlh-ки рендерились и т п создаем сервлет в котором прописываем путь к фтлш-кам , кодировку, то как шаблонный движок должен обрабатывать исключения (рекомендуется отдавать TemplateExceptionHandler.HTML_DEBUG_HANDLER)
```
TemplateExceptionHandler.HTML_DEBUG_HANDLER

Template t = cfg.getTemplate(File file)

template.process(Map data, response.getWriter()); -- рендер
```
и еще кладем всякие ключи-значения из реквеста в data

макросы -- для переиспользования кода
функции 
nested
аннотации? вида 
![[Pasted image 20240211185132.png]]
-- подсказка для среды

восклицательный знак -- если не определено то дефолтное значение которое указано после него
![[Pasted image 20240211185717.png]]
```
if u?has_content
```
методы вызываются через знак вопроса

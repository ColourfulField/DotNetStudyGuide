XSS \(Cross-site scripting\) - одна из базовых атак на сайты, в которых присутствуют любые формы, через которые пользователи могут обмениваться информацией \(например, секция с комментариями\). Если веб-сайт не защищен от XSS атак, то хакер может написать комментарий, содержащий вредоносный Javascript-код и этот код будет выполняться у всех пользователей, просматривающих комментарий.

Для защиты от XSS необходимо провести следующий набор действий:

* Кодировать потенциально вредоносный HTML, чтобы JS-код не смог выполниться. Для этого необходимо экранировать любые опасные символы в потенциально вредоносном тексте \(например, символы '&lt;' и '&gt;', слово 'script'\)
* Фильтровать любой контент пользователей, который вы сохраняете в БД. Под фильтрацией подразумевается исключение из текста всех опасных символов \(\)

Пример того, как этого можно достичь в ASP.NET MVC: [https://docs.microsoft.com/ru-ru/aspnet/core/security/cross-site-scripting](https://docs.microsoft.com/ru-ru/aspnet/core/security/cross-site-scripting)

Крупные Front-end фреймворки вроде Angular или React имеют встроенную защиту от XSS-атак.

XSRF - ещё один популярный вид атак на веб-сайты. Подробнее с методами защиты от них можно ознакомиться тут: [https://habrahabr.ru/post/318748/](https://habrahabr.ru/post/318748/)

А здесь можно почитать о том, как с этим видом атак борется ASP.NET MVC \(английский\): [https://docs.microsoft.com/en-us/aspnet/mvc/overview/security/xsrfcsrf-prevention-in-aspnet-mvc-and-web-pages](https://docs.microsoft.com/en-us/aspnet/mvc/overview/security/xsrfcsrf-prevention-in-aspnet-mvc-and-web-pages)


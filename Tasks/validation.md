# Валидация и обработка ошибок

Валидация входных данных - это процесс проверки корректности данных, которые пользователь вводит в систему или
отправляет на сервер. Цель валидации - предотвращение ошибок и улучшение качества данных, которые хранятся в системе.

В ASP.NET Core есть несколько инструментов валидации, которые могут помочь убедиться в корректности входных данных.
Некоторые из них включают:

- Атрибуты валидации (Data Annotation) - эти атрибуты могут быть применены к модели данных и выполнять проверки на соответствие
определенным правилам. Например, атрибут `[Required]` может быть использован для проверки наличия значения в свойстве
модели.
- [Fluent Validation](https://docs.fluentvalidation.net/en/latest/) - это NuGet пакет, который позволяет определить правила валидации в отдельных классах
валидации и использовать их в приложении.
- Встроенные средства валидации модели - эти средства включают в себя классы, такие как `ModelState` и
`ValidationProblemDetails`, которые позволяют проверять состояние модели и создавать сообщения об ошибках.

## Практика

- Добавьте библиотеку [FluentValidation](https://docs.fluentvalidation.net/en/latest/).
- Реализуйте валидацию при добавления комментария: рейтинг должен принимать значения от 0 до 5; текст комментария должен быть не длиннее 200 символов. 
- Реализуйте валидацию для сущности `Product`: цена товаров должна быть > 0; процент скидки должен принимать значения 0 до 100 не включительно.

## Теория

- [Проверка модели в ASP.NET Core MVC и Razor Pages](https://learn.microsoft.com/ru-ru/aspnet/core/mvc/models/validation?view=aspnetcore-7.0#built-in-attributes).
- [Fluent Validation](https://docs.fluentvalidation.net/en/latest/).
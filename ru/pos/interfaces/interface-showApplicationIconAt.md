## interface.showApplicationIconAt: показать иконку приложения в определенных плейсхолдерах

> Пример запроса:

```javascript
Poster.interface.showApplicationIconAt({
    functions: 'Настройки интеграции',
    order: "Показать popup",
    receiptsArchive: 'Показать закрытый чек'
});
```

Метод добавляет иконку или название приложения в разные места в интерфейсе. При клике на название или иконку приложения сработает событие `applicationIconClicked`.

### Аргументы

Аргумент | Описание
-------- | --------
1-й, places | Объект в котором ключ, место где нужно отображать иконку или название приложения, а значение — заголовок

### Доступные плейсхолдеры

Название | Описание
--------- | -----------
functions | При клике на иконку меню в правом верхнем углу приложения, подходит для функций и настроек общего назначения.
order | При клике на троеточие в нижнем левом углу, на экране заказа. Подходит для функций, которые относятся к текущему заказу
receiptsArchive | При клике на троеточие в архиве чеков. Подходит для функций, которые относятся к текущему заказу
payment | Добавит кнопку на экран оплаты

Пример для плейсхолдера `receiptsArchive`:

<img src="/img/site/docs/app-icon-receipts-archive.jpg" alt="Пример для плейсхолдера receiptsArchive">


Пример для плейсхолдера `payment`:

<img src="/img/site/docs/app-icon-payment.jpg" alt="Пример для плейсхолдера payment">
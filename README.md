# SelsupTask - тестовое задание

Необходимо реализовать на языке Java (можно использовать 11 версию) класс для работы с API Честного знака. Класс должен быть thread-safe и поддерживать ограничение на количество запросов к API. Ограничение указывается в конструкторе в виде количества запросов в определенный интервал времени. Например:
public CrptApi(TimeUnit timeUnit, int requestLimit)
timeUnit – указывает промежуток времени – секунда, минута и пр.
requestLimit – положительное значение, которое определяет максимальное количество запросов в этом промежутке времени.
При превышении лимита запрос должен блокироваться, чтобы не превысить максимальное количество запросов к API и продолжить выполнение, когда ограничение не превышено.

Реализовать нужно единственный метод – Создание документа для ввода в оборот товара, произведенного в РФ. Документ и подпись должны передаваться в метод в виде Java объекта и строки соответственно.
При реализации можно использовать библиотеки HTTP клиента, JSON сериализации. Реализация должна быть максимально удобной для последующего расширения функционала.

Решение должно быть оформлено в виде одного файла CrptApi.java. Все дополнительные классы, которые используются должны быть внутренними.

Документация по работе с API в файле API.pdf.

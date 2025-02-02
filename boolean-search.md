# 1.
Написать запрос для поиска Junior Frontend для Vue или React, но не включать тех у кого указано 0 лет опыта или 1 год опыта
```js
"Junior Frontend" AND (Vue OR React) AND NOT ("Без опыта" OR "Опыт 1 год")
```

# 2.
Создать запрос, который находит Junior либо Senior Frontend разработчика либо developer для фреймфорка Vue либо React
```js
(Junior OR Senior) AND frontend AND (разработчик OR developer) AND (Vue OR React)
```
Модифицируй так, чтобы помимо этих разработчиков еще искался красный либо синий кот либо собака
Условие нахождения котов с собаками выглядит так:
```js
(Красный OR синий) AND (кот OR собака)
```
Необходимо объединить прошлый запрос с текущим:
```js
((Junior OR Senior) AND frontend AND (разработчик OR developer) AND (Vue OR React))
AND
((Красный OR синий) AND (кот OR собака))
```

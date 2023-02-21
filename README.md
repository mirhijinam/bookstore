# Книжный магазин

![bookstore_er_diagram](https://user-images.githubusercontent.com/59884652/220317435-e8b11882-fa45-46a1-9bab-5eb6c09e6f19.jpeg)


## Описание страниц
С любой страницы можно перейти на главную, нажав соответвующую кнопку.

### ***Главная страница***
* Ссылка на страницу с полным списком книг
* Ссылка на страницу с полным списком клиентов
* Ссылка на страницу с полным списком заказов всех клиентов
* Ссылка на страницу с формой оформления заказа

### ***Cтраница с полным списком книг***
* Список книг, добавленных в базу данных с возможностью фильтровать по жанрам, авторам и др. характеристикам.
* Переход на страницу книги с дополнительной информацией при нажатии на ее ID
* Форма для поиска книги по названию, перенаправляющая на страницу книги с дополнительной информацией
* Ссылка на форму для добавления книги
    #### _Страница книги_
    * Содержащаяся информация: ID, название, автор, жанр, количество экземпляров, стоимость
    * Ссылка на форму для редактирования данных о книге
    * Кнопка для удаления книги

### ***Cтраница с полным списком клиентов***
* Список клиентов, добавленных в базу данных.
* Переход на страницу клиента с информацией о его заказах при нажатии на его ID
* Форма для поиска клиента по ФИО, перенаправляющая на страницу клиента с информацией о его заказах
* Ссылка на форму для регистрации клиента
    #### _Страница клиента_
    * Содержащаяся информация: ID, ФИО, список оформленных заказов
    * Ссылка на форму для редактирования данных о клиенте
    * Кнопка для удаления клиента

### ***Страница с полным списком заказов***
* Список заказов, добавленных в базу данных.
* Переход на страницу заказа с дополнительной информации при нажатии на его ID
    #### _Страница заказа_
    * Содержащаяся информация: ID заказа, ID клиента, IDs книг, статус, стоимость
    * Ссылка на форму для редактирования информации о заказе

### ***Ссылка на страницу с формой оформления заказа***
* Форма ввода информации о клиенте
* Форма ввода информации о книгах
* Кнопка для сохранения заказа в БД

<img width="1185" alt="bookstore_diagram_site" src="https://user-images.githubusercontent.com/59884652/220226610-3f3c9391-762b-45e2-bc92-dd60fcfbfe34.png">


## Сценарии использования

### ***Получение списка книг по жанрам, авторам и др. характеристикам***
* Перейти на главную страницу
* Перейти на страницу с полным списком книг
* Использовать параметры фильтрации при необходимости
 
### ***Получение данных о наличии и цене книг*** 
* Перейти на главную страницу
* Перейти на страницу с полным списком книг
* Найти книги в списке(при необходимости используя параметры фильтрации) или используя форму для поиска
* Нажать на ID клиента, чтобы перейти на страницу книги с необходимой информацией

### ***Оформление заказа***
* Перейти на главную страницу
* Перейти по страницу с формой оформления заказа
* Заполнить необходимые поля
* Нажать кнопку "Сохранить"

### ***Проверка статуса заказа***
* Перейти на главную страницу
* Перейти на страницу с полным списком заказов всех клиентов
* Нажать на ID интересующего заказа, чтобы перейти на страницу заказа с необходимой информацией

### ***Изменение статуса заказа***
* Перейти на главную страницу
* Перейти на страницу с полным списком заказов всех клиентов
* Нажать на ID интересующего заказа, чтобы перейти на страницу заказа
* Перейти на страницу с формой редактирования заказа
* Внести необходимые изменения
* Нажать кнопку "Сохранить"

### ***Добавление клиента***
* Перейти на главную страницу
* Перейти на страницу с полным списком клиентов
* Перейти на страницу с формой регистрации клиента
* Заполнить необходимые поля
* Нажать кнопку "Сохранить"

### ***Удаление клиента***
* Перейти на главную страницу
* Перейти на страницу с полным списком клиентов
* Найти клиента в списке или используя форму для поиска
* Нажать на ID клиента, чтобы перейти на страницу клиента
* Нажать кнопку "Удалить"

### ***Чтение данных о клиенте***
* Перейти на главную страницу
* Перейти на страницу с полным списком клиентов
* Найти клиента в списке или используя форму для поиска
* Нажать на ID клиента, чтобы перейти на страницу клиента с необходимой информацией

### ***Редактирование данных о клиенте***
* Перейти на главную страницу
* Перейти на страницу с полным списком клиентов
* Найти клиента в списке или используя форму для поиска
* Нажать на ID клиента, чтобы перейти на страницу клиента
* Перейти на страницу с формой редактирования данных о клиенте
* Внести необходимые изменения
* Нажать кнопку "Сохранить"

### ***Добавление книги***
* Перейти на главную страницу
* Перейти на страницу с полным списком книг
* Перейти на страницу с формой добавления книги
* Заполнить необходимые поля
* Нажать кнопку "Сохранить"

### ***Удаление книги***
* Перейти на главную страницу
* Перейти на страницу с полным списком книг
* Найти книги в списке(при необходимости используя параметры фильтрации) или используя форму для поиска
* Нажать на ID книги, чтобы перейти на страницу книги
* Нажать кнопку "Удалить"

### ***Чтение данных о книге***
* Перейти на главную страницу
* Перейти на страницу с полным списком книг
* Найти книги в списке(при необходимости используя параметры фильтрации) или используя форму для поиска
* Нажать на ID книги, чтобы перейти на страницу книги с необходимой информацией

### ***Редактирование данных о книге***
* Перейти на главную страницу
* Перейти на страницу с полным списком книг
* Найти книги в списке(при необходимости используя параметры фильтрации) или используя форму для поиска
* Нажать на ID книги, чтобы перейти на страницу книги
* Перейти на страницу с формой редактирования данных о книге
* Внести необходимые изменения
* Нажать кнопку "Сохранить"

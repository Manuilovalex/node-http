# HTTP-сервер на Node.js

Это базовый HTTP-сервер на Node.js, который обрабатывает GET и POST запросы. Сервер возвращает статические HTML-страницы в ответ на GET-запросы и обрабатывает данные POST-запросов.

## Установка
1. Клонировать репозиторий.<br>
2. Убедиться, что установлена Node.js (версия 12 или выше).<br>
3. Установить любые дополнительные зависимости<br>
yarn<br>
npm install

## Запуск сервера 
yarn start<br>npm start


## Сервер будет прослушивать на порту 3000.

## Маршруты
GET /: Главная страница.<br>
GET /text: Простой текст в ответе.<br>
GET /json: JSON со списком задач (todos).<br>
GET /todos: HTML-страница со списком задач.<br>
GET /form: HTML-форма для добавления новой задачи.<br>
POST /todos: Принимает данные POST и добавляет новую задачу.<br>

## Обработка POST-запросов
Сервер обрабатывает POST-запросы в форматах application/x-www-form-urlencoded и application/json. Если данные некорректные, возвращается ошибка 400.

## Тестирование
Для тестирования используйте инструменты, такие как Postman.<br>

GET /: Открыть в браузере.<br>
GET /todos: Проверить в браузере или с помощью Postman.<br>
POST /todos: Отправить POST-запрос через Postman.
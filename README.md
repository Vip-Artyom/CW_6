### Coursework №6

##### В этой работе мы создаем свой сайт объявлений.

На сайте можно посмотреть список всех объявлений, одно объявление детально. Также можно создать, обновить или удалить объявление.

Работа с пользователем реализована через djoser.

Объявления могут содержать комментарии, для них также реализован CRUD.

Фронтэнд доступен по адресу: http://127.0.0.1:3000/
___
Для запуска контейнера и наполнения базы необходимо в терминале выполнить следующие команды:
```
docker-compose up --build -d (из директории market_postgres/)
python ./manage.py migrate (из директории skymarket/)
python ./manage.py loaddata fixtures/ad.json fixtures/comments.json fixtures/users.json (из директории skymarket/)
```
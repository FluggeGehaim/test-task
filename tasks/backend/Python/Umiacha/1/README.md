# Задание 1.
## Как запустить?
* Клонируйте данный проект туда, где хотите развернуть приложение.
* Переименуйте '.env.example' в '.env' и перепишите константы окружения на ваше усмотрение:
    + DJANGO_SECRET_KEY -- CSRF-токен, который генерируется приложением Django при создании.
    Вы можете сгенерировать свой на соответствующих сайтах.
    + DJANGO_DEBUG -- режим приложения Django: перед размещением сервиса
    в открытом доступе следует изменить значение на False.
    + DJANGO_HOSTS -- список хостов, с которых можно подключиться к приложению.
    Если у вас есть свой домен, то для доступа к приложению через него, нужно
    добавить доменное имя в этот список по аналогии с уже приведенными.
* Из текущей директории (где находится этот README.md) выполнить следующее:
```
docker compose up -d
```
P.S.: если у вас недостаточно прав для выполнения команды выше, то:
```
sudo docker compose up -d
```
* Если вы ничего не меняли в .env, то теперь сайт доступен по http://127.0.0.1:8000.

## Что есть?
С возможностями сервиса можно ознакомиться, если запустить его и перейти по ссылкам:
* Swagger: http://127.0.0.1:8000/swagger/
* Redoc: http://127.0.0.1:8000/redoc/
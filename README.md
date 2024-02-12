# Taski

### Описание проекта Taski
Taski - Это трекер задач, где вы можете добавлять, изменять и удалять задачи.

### Cписок используемых технологий

- Django
- React
- pytest
- djangorestframework
- Docker

### Как запустить проект:
`git clone git@github.com:SerVik888/kittygram_final.git` -> клонировать репозиторий

**При помощи docker**\
    Перед началом нужно установить и запустить Docker.

    `docker-compose up` -> запустить Docker Compose
    `docker-compose stop` -> остановить Docker Compose

**Без docker**

Запуск backend

`cd backend` -> перейти в папку

* Если у вас Linux/macOS\
    `python3 -m venv env` -> создать виртуальное окружение\
    `source env/bin/activate` -> активировать виртуальное окружение\
    `python3 -m pip install --upgrade pip` -> обновить установщик\
    -> Перейдите в папку backend\
    `pip install -r requirements.txt` -> установить зависимости из файла requirements.txt\
    `python3 manage.py migrate` -> выполнить миграции\
    `python3 manage.py createsuperuser` -> создать суперпользователя\
    `python3 manage.py runserver` -> запустить проект

* Если у вас windows\
    `python -m venv venv` -> создать виртуальное окружение\
    `source venv/Scripts/activate` -> активировать виртуальное окружение\
    `python -m pip install --upgrade pip` -> обновить установщик\
    -> Перейдите в папку backend\
    `pip install -r requirements.txt` -> установить зависимости из файла requirements.txt\
    `python manage.py migrate` -> выполнить миграции\
    `python manage.py createsuperuser` -> создать суперпользователя\
    `python manage.py runserver` -> запустить проект

Запуск frontend нужно выполнять в другом терминале

`cd frontend` -> перейти в папку\
`npm i` -> установить зависимости\
`npm run start` -> запуск приложения


### Как заполнить файл .env:
В проекте есть файл .env.example заполните свой по аналогии.

`POSTGRES_DB` - название базы\
`POSTGRES_USER` - пользователь базы\
`POSTGRES_PASSWORD` - пароль к базе\
`DB_NAME` - имя базы\
`DB_HOST` - имя контейнера, где запущен сервер БД\
`DB_PORT` - порт, по которому Django будет обращаться к базе данных
`DB_SQLIGTH` - если эта переменная есть используется база sqlite если нет то postgres


Автор:
Сафонов Сергей https://github.com/SerVik888 [sergey_safonov86@inbox.ru](mailto:sergey_safonov86@inbox.ru)

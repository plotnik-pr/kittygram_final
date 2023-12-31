# Kittygram

### Сервис для владельцев и просто любителей котиков.

Проект, который позволяет делиться своими котиками и смотреть чужих.
Всё это в удобном редакторе, где вы можете загрузить фотографию, имя, дату рождения, выборать цвет и достиженя ваших любимцев.
Для добавления котика нужно зарегистрироваться. 
Проект систематизирован в рамках учебного курса по Python от Яндекс.Практикум.


### Технологии

- Python
- JavaScript
- Gunicorn
- Nginx
- Node.js


### Установка проекта.

Приложение запускается при помощи платформы Docker.
Скачайте файл 'docker-compose.production.yml' из репозитория 'github.com/plotnik-pr/kittygram_final' и добавьте на ваш сервер в любую пустую папку.
Перед запуском добавьте необходимые переменные окружения в файл '.env' в папке с проектом:
```
POSTGRES_DB=kittygram
POSTGRES_USER=kittygram_user
POSTGRES_PASSWORD=kittygram_password
DB_NAME=kittygram
DB_HOST=db
DB_PORT=5432
SECRET_KEY = 'SECRET_KEY'
DEBUG = 'True'
ALLOWED_HOSTS = 'HOST'
```
Для запуска проекта выполните команду 
```
sudo docker compose -f docker-compose.production.yml up --build 
```

### Доступные эндпоинты

- Ваш IP - главная страница проекта
- Ваш IP/admin/ - страница администратора(суперпользователя)
Вместо Ваш_IP может быть использован домен.


### Авторы

Программисты Яндекс Практикум, Плотник Ульяна (https://github.com/plotnik-pr)
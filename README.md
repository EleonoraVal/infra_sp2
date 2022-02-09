### Описание проекта:

Yamdb:

```
Проект YaMDb собирает отзывы пользователей на различные произведения. Произведения делятся на жанры и категории.
```

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/EleonoraVal/api_yamdb.git
```

```

cd api_yamdb
```

cd infra
```
Разверните контейнеры:
```

docker-compose up -d --build

```

Выполнить миграции:

```
docker-compose exec web python manage.py migrate
```
Создать суперпользователя:
```
docker-compose exec web python manage.py createsuperuser
```
Собрать статику:
```
docker-compose exec web python manage.py collectstatic --no-input
```

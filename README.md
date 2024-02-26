# base setup with user and token auth fully tested

## comands

### run flake8 linting
    docker-compose run --rm app sh -c "flake8"

### install Django
    docker-compose run --rm app sh -c "django-admin startproject app ."

### run tests
    docker-compose run --rm app sh -c "python manage.py test"

### migrations
    docker-compose run --rm app sh -c "python manage.py makemigrations"

    docker-compose run --rm app sh -c "python manage.py migrate"


### clear docker volume (clears database)
    docker volume ls
    docker volume rm recipe-app-api_dev-db-data


### create super user
    docker-compose run --rm app sh -c "python manage.py createsuperuser"


### openapi swagger 
    http://localhost:8000/api/docs/
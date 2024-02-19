## comands

### run flake8 linting
    docker-compose run --rm app sh -c "flake8"

### install Django
    docker-compose run --rm app sh -c "django-admin startproject app ."

### run tests
    docker-compose run --rm app sh -c "python manage.py test"
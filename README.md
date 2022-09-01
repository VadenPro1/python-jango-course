
``` 
# Run linting
dc run --rm app sh -c "flake8"

# Run tests
dc run --rm app sh -c "python manage.py test"

#Install sub project
dc run --rm app sh -c "django-admin startproject app ."

#Install core project
docker-compose run --rm app sh -c "python manage.py startapp recipe"

#Create superuser
docker-compose run --rm app sh -c "python manage.py createsuperuser"

#Work with migrations
docker-compose run --rm app sh -c "python manage.py migrate"
docker-compose run --rm app sh -c "python manage.py makemigrations"
docker-compose run --rm app sh -c "python manage.py showmigrations"
```

``` 
# Run linting
dc run --rm app sh -c "flake8"

# Run tests
dc run --rm app sh -c "python manage.py test"

#Install jango project
dc run --rm app sh -c "django-admin startproject app ."

#Install core project
docker-compose run --rm app sh -c "python manage.py startapp core"
```
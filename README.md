# python-recipe-app-api
python project for recipe api

# build the docker

docker-compose build

# django admin 
docker-compose run app sh -c "django-admin.py startproject app ."

# run test cases with linting (flake8)

docker-compose run app sh -c "python manage.py test && flake8"

# create core app
- this core app will contain the migrations, db config and other configurations for the project

docker-compose run app sh -c "python manage.py startapp core"

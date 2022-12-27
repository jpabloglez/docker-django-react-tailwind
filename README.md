# React (Tailwind) + Django

## Setup
* Starting  from base_config branch
Run next commands:
```
docker-compose up -d --build
```

## Configuration

    |--app
    |--app/backend
    |--app/frontend

## Backend

## Setup 
After image is build and running
```
docker exec -it backend-app django-admin startproject backend
```
Once configured our project let's create our first django-app (users)
```
docker exec -it django-app bash 
cd app && python manage.py startapp users
```
Then apply migrations and create superuser
```
docker exec -it django-app bash 
cd app && python manage.py makemigrations 
python manage.py migrate
python manage.py cretesuperuser
```
## Setup 
* Starting from master or main/dev branch
Run next:
```
docker-compose build
docker-compose up -d
```
Create new django-app using:
```
docker exec -it django-app python manage.py migrate
```

## Tailwind

## References:

* [React vs. Vue (Exact Todo App) By Example](https://medium.com/js-dojo/react-vs-vue-exact-todo-app-comparison-by-example-14cc56efc5e5)

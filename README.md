# Docker-Django-Pipenv-MySQL
Awesome development environment setup
Docker + Pipenv + Django Rest Framework + MySQL AWESOME TUTORIAL: https://medium.com/zeitcode/a-simple-recipe-for-django-development-in-docker-bonus-testing-with-selenium-6a038ec19ba5

### Pipenv basics
https://www.techiediaries.com/pipenv-tutorial/
pipenv install getenv

Docker Commands: coming soon



### Setting up pipenv:
Install pipenv: 
pip install pipenv

### Create pipenv envelope:
pipenv shell --three

### Install dependencies
pipenv install django
pipenv install djangorestframework
pipenv install dj-database-url
pipenv install getenv


### Setting up Django:
Create the backend directory:
django-admin.py startproject backend


### Database installation, Creation, and Configuration:
Install mysql: https://stackoverflow.com/questions/41645309/mysql-error-access-denied-for-user-rootlocalhost

### Start the mysql server: 
service mysql start
### Note, command to stop mysql server below:
service mysql stop
### Note:  command to check if server is running:
service mysql status

### Setup a user:
 ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'akirademoss’';
mysql -u root -p

### Create a database:
CREATE DATABASE django_db;

### Change settings.py to recognize environment variables:
Add this to top: import dj_database_url
Add this below: DATABASES = {'default': dj_database_url.config()}





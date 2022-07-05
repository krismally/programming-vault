# How to set up Basic Django Dev Environment
### Basic Setup 
1. CREATE DATABASE *database_name* in psql shell
2. Windows - run `python -m pipenv shell` in /django_env directory, Mac - run `pipenv shell` in /django_env directory
3. cd into where you want to store django project
4. run `django-admin startproject [project_name]` 
5. cd into project directory and run `code .` to open VS Code
6. change interpreter to the pipenv virtual environment via command prompt or via shortcut (in between 'Python' and 'Go Live' on footer)
7. open VS code bash terminal
	1. Make sure you see (django_env), if not trash terminal and reopen 
8. Windows - run `py manage.py startapp main_app` Mac - run `python manage.py startapp main_app`
9. Open settings.py file in your project_name directory
10. Add `'main_app',` to `INSTALLED_APPS` in settings.py (line 34)
11. In terminal - Windows - run `py manage.py runserver` Mac - run `python manage.py runserver`
12. Connect to database
	1. Starting on line 79 in settings.py change to `'ENGINE': 'django.db.backends.postgresql', 'NAME': 'catcollector',
		1.  if error saying 'no password supplied' also add ```
			'USER': 'postgres',
	        'PASSWORD': '[postgresql password]',
	        'HOST': 'localhost',
	        'PORT': '5432', ```
13. In terminal - Windows - run `py manage.py migrate` Mac - run `python manage.py migrate`

### Basic URL Setup
1. In main_app directory - create urls.py file
2. Include in project directory's urls.py (not main_app directory), file should look like: 
	1. ```from django.contrib import admin
		from django.urls import path, include
		
		urlpatterns = [
			path('admin/', admin.site.urls),
			path('', include('main_app.urls')),
		]``` 
3.  Close project directory's urls.py
4. Open `main_app/urls.py` 
5. Add boilerplate for URLs
	1. ```from django.urls import path
		from . import views

		urlpatterns = [

		]``` 

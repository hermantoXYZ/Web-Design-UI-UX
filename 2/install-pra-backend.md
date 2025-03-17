---
hidden: true
---

# Install Pra Backend

## Django Start Project Guide

### 1. Install Django

```sh
python --version
```

```sh
pip install django
```

Verify the installation:

```sh
django-admin --version
```

### 2. Create a Django Project

```sh
django-admin startproject myproject
```

```
myproject/
    manage.py
    myproject/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
```

### 3. Run the Development Server

```sh
cd myproject
```

```sh
python manage.py runserver
```

You should see output like:

```
Starting development server at http://127.0.0.1:8000/
```

Open your browser and visit `http://127.0.0.1:8000/` to see the default Django welcome page.

### 4. Create a Django App

Inside your project directory, run:

```sh
python manage.py startapp myapp
```

This creates a directory structure like this:

```
myapp/
    __init__.py
    admin.py
    apps.py
    models.py
    tests.py
    views.py
    migrations/
        __init__.py
```

### 5. Register the App in Settings

Open `settings.py` and add your app to the `INSTALLED_APPS` list:

```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'myapp',
]
```

### 6. Define Models

Open `models.py` in `myapp` and define a model:

```python
from django.db import models

class Post(models.Model):
    title = models.CharField(max_length=200)
    content = models.TextField()
    created_at = models.DateTimeField(auto_now_add=True)
```

Run migrations to apply the model to the database:

```sh
python manage.py makemigrations
python manage.py migrate
```

### 7. Create a Superuser

To access the Django admin panel, create a superuser:

```sh
python manage.py createsuperuser
```

Follow the prompts to set up a username and password.

### 8. Run the Server and Access Admin Panel

Start the server again:

```sh
python manage.py runserver
```

Visit `http://127.0.0.1:8000/admin/` and log in with your superuser credentials.

### 9. Create Views and URLs

Define a simple view in `views.py`:

```python
from django.http import HttpResponse

def home(request):
    return HttpResponse("Hello, Django!")
```

Map the view to a URL in `urls.py`:

```python
from django.urls import path
from myapp.views import home

urlpatterns = [
    path('', home, name='home'),
]
```

### 10. Test Your Application

Restart the server and visit `http://127.0.0.1:8000/`. You should see `Hello, Django!` displayed.

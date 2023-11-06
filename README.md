# django-mysite
Getting started with Django, created a polling application

django-admin startproject mysite

python manage.py runserver

python manage.py runserver 8080

python manage.py runserver 0.0.0.0:8000

python manage.py startapp polls

python manage.py makemigrations polls

python manage.py migrate

python manage.py sqlmigrate polls 0001

python manage.py check

python manage.py shell

python manage.py createsuperuser

### Building your package (run from inside django-polls)
- This creates a directory called dist and builds your new package, django-polls-0.1.tar.gz.
```commandline
python setup.py sdist
```

### Using your own package
1. To install the package, use pip (you already installed it, right?):
    ```commandline
    python -m pip install --user django-polls/dist/django-polls-0.1.tar.gz
    ```
2. With luck, your Django project should now work correctly again. Run the server again to confirm this.
3. To uninstall the package, use pip:
    ```commandline
    python -m pip uninstall django-polls
    ```

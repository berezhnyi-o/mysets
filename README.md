# Basics

Before working with a project add a new line to your `/etc/hosts`

    127.0.0.1    myset.local

### How to run local development server

    ./manage.py runserver

### How to run Celery worker

    DJANGO_SETTINGS_MODULE=myset.settings.development celery -A myset worker -B --loglevel=info

### How to run unit tests

    DJANGO_SETTINGS_MODULE=myset.settings.testing ./manage.py test

---
layout: post
---

# Django заметки

после создания проекта внутри появятся файлы.



```
manage.py - консольная утилита
project-name - папка с названием проекта
----
	|- __init__.py - файл, чтобы сообщить питону что данная директория является пакетом	|- settings.py - настройки	|- urls.py - корневая URL привязка	|- wsgi.py - файл для вебсерверов

```

что внутри settings.py

```INSTALLED_APPS``` - список установленных приложений
```DATABASES``` - настройка для соединения с БД

Как сделать, чтобы приложения были внутри папки apps в нашем проекте.

Создаем приложение
```
python manage.py startapp custom_app_name
```

В файл settings.py дописываем небольшой код. Будет выглядеть типа так

```
...
import os, sys

# Build paths inside the project like this: os.path.join(BASE_DIR, ...)

BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))

PROJECT_ROOT = os.path.dirname(__file__)
sys.path.insert(0, os.path.join(PROJECT_ROOT, '_apps_'))
...

```

`+ Внутри проекта создаем папку apps, а внутрь закидываем наше созданное приложение.


```
manage.py

project-name
	|- __init__.py	|- settings.py	|- urls.py	|- wsgi.py
	|-apps
		|-custom_app_name
			|- migrations
			|-_init_.py
			|- admin.py - тут будем указывать, какие данные будут редактироваться в админке
			|- apps.py - указываем конфиг нашего приложения
			|- models.py - указываем модель нашего приложения
			|- test.py - файл, в котором можно прописывать тесты
			|- views.py - тут прописываем логику приложения
			|- urls.py (сами создаем) - url привязка локальная для данного приложения
			|- forms.py (сами создаем) - для работы с формами

```

## Как создать страницу (роутинг в Django)

## Модели

В файле model.py - мы объясняем джанге из чего состоит наше приложение. Что ей хранить в БД

# Миграции 
Такой метод благодаря которому джанго понимает какие изменения и когда он вносит в БД, чтобы можно было откатываться и тп

Чтобы создать миграцию нужно

1. Добавить наше приложение в файл settings.py в секцию installedAPPS

будет выглядеть типа так

```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'atricles.apps.AtriclesConfig', # наше добавленное приложение
]
```

2. Создать и запустить миграцию

```bash
$ python manage.py makemigrations your_app_name
Migrations for 'articles':
  myfirst/apps/articles/migrations/0001_initial.py
    - Create model Article
    - Create model Comment
$ python manage.py migrate
```

## ORM Django 





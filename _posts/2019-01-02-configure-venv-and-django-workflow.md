---
layout: post
title: "Настройка venv и Django Workflow"
categories: django
---


1) Проверим текущую версию Python.

```
$ python --version
Python 3.7.3
```

2) Создаем директорию с нашим проектом и перейдем в нее.

```
$ mkdir project_folder_name
$ cd project_folder_name
```

3) Создаем virtual environment

```
$ python -m venv venv
```

4) Чтобы запустить venv, нужно из родительского каталога запустить

```
$ source venv/bin/activate
```

5) Установим туда Django

```
$ pip install Django==2.1.5
```
Если устанавливаем Flask, то используем

```
$ pip install flask
```

6) Создадим файлы стартового проекта

```
$ django-admin startproject my_project
```

7) Запустим Django

```
$ cd my_project
$ python manage.py runserver
```
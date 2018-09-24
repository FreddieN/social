<div align="center">
  <br>
  <img
    alt="Sugar Social"
    src="https://image.ibb.co/hX7JhU/sugarsocial.png"
    width=500px
  />
  <br/>
  <h1>Sugar Labs Social</h1>
  <strong>Learn | Create | Share</strong>
</div>
<br/>


<p align="center">
  <a href="https://www.djangoproject.com/">
    <img src="https://img.shields.io/badge/Django-v2.0.6-brightgreen.svg" alt="django version"/>
  </a>
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Python-v3-orange.svg" alt="python version"/>
  </a>
  <a href="https://www.postgresql.org/">
    <img src="https://img.shields.io/badge/Database-postgresql-blue.svg" alt="database postgresql"/>
  </a>
</p>

Welcome to the Sugar Labs Social codebase. We are so excited to have you. With your help, we can build out Sugar Labs Social to be more stable and better.


## What is Sugar Labs Social?
A Platform for sugar users/instructors/developers/teachers/parents to explore/discuss/share about Projects/softwares/activities/blogs/posts related to Sugar Labs|OLPC ❤️



## Table of Contents


- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installing_Prerequisites](#installingprerequisites)
    - [Setting_up_postgresql_database](#settinguppostgresqldatabase)
    - [Creating Virtual Enviornment](#creating-virtual-enviornment)
    - [Installing and Running the project](#installing-and-running-the-project)
- [:boom: BOOM!](#boom-boom)









# Getting Started


* clone the project in your local computer
```
$ git clone https://github.com/avinashbharti97/SugarLabs_Social.git
```

## Prerequisites



```
- python3
- pip3
- virtualenvwrapper
- postgresql
```

## Installing_Prerequisites

```
$ sudo apt-get update
$ sudo apt-get install python3 python3-pip virtualenvwrapper python-dev libpq-dev postgresql postgresql-contrib
```

## Setting_up_postgresql_database
>keep the value of database name, username and password same,
>else change the config respectively of settings.py in Project_SLS dir.

```
$ sudo su - postgres
```
> You should now be in a shell session for the postgres user. Log into a Postgres session by typing:
```
psql
```
> creating the database
```
CREATE DATABASE database;
```
*Remember to end all commands at an SQL prompt with a semicolon.*
> create the user with password
```
CREATE USER username WITH PASSWORD 'password';
```
> one more step
```
GRANT ALL PRIVILEGES ON DATABASE database TO username;
```
> exit the shell
```
\q
```
```
exit
```


## Creating Virtual Enviornment
* move to the cloned project directory
```
$ virtualenv -p /usr/bin/python3 env
```
activate the virtualenv
```
$ source env/bin/activate
```
you should see (env) in the begining, something like this.
```
(env) avinash@engine:/media/avinash/raw/development/SugarLabs_Social$
```


## Installing and Running the project



```
$ pip install -r requirements.txt
```
```
$ cd Project_DIR
```
```
$ python manage.py makemigrations
```
>if any prompt choose option 2
```
$ python manage.py migrate
```
> ignore some errors
```
$ python manage.py runserver
```
you will see something like This
```
Performing system checks...

System check identified no issues (0 silenced).
June 07, 2018 - 11:12:23
Django version 1.11.13, using settings 'Project_SLS.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
```

Redirect at the link shown.
# :boom: BOOM!

﻿# **api\_final**
**Описание.**  Проект API для Yatube 

**Как запустить проект:**

***Клонировать репозиторий и перейти в него в командной строке:***

git clone <https://github.com/momtheprogram/api_final_yatube.git>

cd api\_final\_yatube

***Cоздать и активировать виртуальное окружение:***

python3 -m venv env

source env/bin/activate

***Установить зависимости из файла requirements.txt:***

python3 -m pip install --upgrade pip

pip install -r requirements.txt

***Выполнить миграции:***

python3 manage.py migrate

***Запустить проект:***

python3 manage.py runserver


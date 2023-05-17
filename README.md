# **api final**
###Описание.
Проект API для Yatube. Через этот интерфейс могут работать 
мобильное приложение или чат-бот; 
через него же можно передавать данные 
в любое приложение или на фронтенд.

### Как запустить проект:

***Клонировать репозиторий и перейти в него в командной строке:***

```bash
git clone <https://github.com/momtheprogram/api_final_yatube.git>

cd api_final_yatube
``` 


***Cоздать и активировать виртуальное окружение:***


```bash
python3 -m venv env

source env/bin/activate
``` 


***Установить зависимости из файла requirements.txt:***

```bash
python3 -m pip install --upgrade pip

pip install -r requirements.txt
``` 

***Выполнить миграции:***

```bash
python3 manage.py migrate
``` 

***Запустить проект:***

```bash
python3 manage.py runserver
```


###Пример запроса к API и ответа от сервера.
Получить список всех публикаций:\
запрос

```postman
GET http://127.0.0.1:8000/api/v1/posts/
```
ответ
```json
{
  "count": 123,
  "next": "http://api.example.org/accounts/?offset=400&limit=100",
  "previous": "http://api.example.org/accounts/?offset=200&limit=100",
  "results": [
    {
      "id": 0,
      "author": "string",
      "text": "string",
      "pub_date": "2021-10-14T20:41:29.648Z",
      "image": "string",
      "group": 0
    }
  ]
}
```

### Использованые технологии:
 - Django
 - DRF
 - Python
 - SQLite
 
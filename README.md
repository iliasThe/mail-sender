# mail-sender
Написать на Python 2.7 (это не опечатка, мы действительно работаем на Python 2.7. Если вы не готовы работать в данной версии, напишите пожалуйста в нашем с вами чате на HH.ru. Спасибо!)
/ Django небольшой сервис отправки имейл рассылок.
Возможности сервиса:
 1. Отправка рассылок с использованием html макета и списка подписчиков.
 2. Отправка отложенных рассылок.
 3. Использование переменных в макете рассылки. (Пример: имя, фамилия, день рождения из списка подписчиков)
 4. Отслеживание открытий писем.
Отложенные отправки реализовать при помощи Celery.

P.S.: Способ хранения макетов писем и списков подписчиков на усмотрение исполнителя.

           
           
1. Склонировать репозиторий с Github:

````
git clone https://github.com/iliasThe/mail-sender.git
````

2. Запускаем необходимые:

````
python manage.py runserver; python -m celery -A mailing_app worker -B --loglevel=info
````
 
3. Установка зависимостей:

```
pip install -r requirements.txt
```

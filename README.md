# Init
1. Оклжчить слежение git за конфиг файлами
```
$ ./notfollow.sh
```

2. Изменить файл functions/authData.py для отправки оповещения в ВК
```
authData = dict(email = "Ваш логин vk", password = "Ваш пароль вк!")
```

3. Изменить файл по желанию crontask.sh
```
cd /путь/до/каталога/этой/программы #(/home/python/pbox)
```

4. Добавить задачу в крон, запись в конец файла
```
$ sudo nano /etc/crontab
```
Строку:
```
* * * * *  silent /путь/до/каталога/crontab.sh >> /путь/до/каталога/cron.log
```
Это будет  запускать задачу парсинга сайта кажду гребанную минуту

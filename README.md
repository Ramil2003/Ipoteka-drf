# Высчитывание ипотеки

----

### Пользовательский сценарий
Клиент вводит следующие данные:
1. Стоимость объекта недвижимости, в рублях без копеек. Тип данных: integer
2. Первоначальный взнос, в рублях без копеек. Тип данных: integer
3. Срок, в годах. Тип данных: integer

В ответ ему приходит массив с объектами ипотечных предложений. В каждом объекте есть следующие данные:
1. Наименование банка. Тип данных: string
2. Ипотечная ставка, в процентах. Тип данных: float
3. Платеж по ипотеке, в рублях без копеек.  Тип данных: integer

----

Создаем виртуальное окружение и активируем
```
python3 -m venv venv
```
```
source venv/bin/activate
```

Устанавливаем зависимости
```
pip install -r requirements.txt
```

## Локальный запуск приложения

Создаем супер юзера
```
python3 manage.py createsuperuser
```

Делаем миграции и запускаем
```
python3 manage.py makemigrations
```
```
python3 manage.py migrate
```
```
python3 manage.py runserver
```

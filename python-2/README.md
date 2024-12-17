
# Домашнее задание к лекции 2.«Условные конструкции. Операции сравнения»

## Задача №1
Задачи на [hackerrank](https://www.hackerrank.com/domains/python):  
Решить задачу на hackerrank ["Python If-Else"](https://www.hackerrank.com/challenges/py-if-else/problem).  
![image](https://github.com/user-attachments/assets/cfeefb9b-2932-4171-9815-752210068d83)


## Задача №2
На лекции мы рассматривали пример для военкомата. Сейчас мы знаем про его рост. Расширить это приложение следующими условиями:
1. Проверка на возраст призывника.
2. Количество детей.
3. Учится ли он сейчас.
Ответ:
```py
height = input("Введите рост призывника: ")
age = input("Введите возраст призывника: ")
children = input("Введите количество детей призывника: ")
study = input("Учится ли призывник сейчас? (д/н): ")
if 18 <= int(age) <= 27:
  if int(children) < 2:
    if study == "н":
      if int(height) < 170:
        print("В танкисты")
      elif int(height) < 185:
        print("На флот")
      elif int(height) < 200:
        print("В десантники")
      else:
        print("В другие войска")
    else:
      print("Не годен")
  else:
    print("Не годен")
else:
  print("Не призывной возраст")
```
```
Введите рост призывника: 182
Введите возраст призывника: 21
Введите количество детей призывника: 0
Учится ли призывник сейчас? (д/н): н
На флот
```

## Задание №3
Разработать приложение для определения знака зодиака по дате рождения.  
Пример:  
```
Введите месяц: март
Введите число: 6

Вывод:
Рыбы
```
Решение:
```py
month = int(input("Введите месяц рождения: "))
day = int(input("Введите день рождения: "))
if month == 1:
  if day <= 20:
    print("Козерог")
  else:
    print("Водолей")
elif month == 2:
  if day <= 18:
    print("Водолей")
  else:
    print("Рыбы")
elif month == 3:
  if day <= 20:
    print("Рыбы")
  else:
    print("Овен")
elif month == 4:
  if day <= 20:
    print("Овен")
  else:
    print("Телец")
elif month == 5:
  if day <= 21:
    print("Телец")
  else:
    print("Близнецы")
elif month == 6:
  if day <= 21:
    print("Близнецы")
  else:
    print("Рак")
elif month == 7:
  if day <= 22:
    print("Рак")
  else:
    print("Лев")
elif month == 8:
  if day <= 23:
    print("Лев")
  else:
    print("Дева")
elif month == 9:
  if day <= 23:
    print("Дева")
  else:
    print("Весы")
elif month == 10:
  if day <= 23:
    print("Весы")
  else:
    print("Скорпион")
elif month == 11:
  if day <= 22:
    print("Скорпион")
  else:
    print("Стрелец")
elif month == 12:
  if day <= 21:
    print("Стрелец")
```
```
Введите месяц рождения: 6
Введите день рождения: 13
Близнецы
```

## Задание №4
К следующей лекции прочитать про циклы [for](https://foxford.ru/wiki/informatika/tsikl-for-v-python) и
 [while](https://foxford.ru/wiki/informatika/tsikl-while-v-python).

---


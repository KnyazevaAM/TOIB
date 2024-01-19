# Отчет по ПР-2 "Идентификация и аутентификация" ББМО-01-23 Князевой А.М. 


## Шаги выполнения


# Шаг 1


Создаем суперпользователя Super-Knyazeva.A.M
 sudo useradd Super-Knyazeva.A.M
 
 sudo usermod -a -G sudo Super-Knyazeva.A.M
 
 passwd Super-Knyazeva.A.M
 
![1]()


# Шаг 2

Создаем группу group-BBMO-01-23.

sudo groupadd BBMO-01-23

sudo usermod -aG BBMO-01-23 Super-Knyazeva.A.M


![2]()


# Шаг 3

Создаем обычного пользователя User-Knyazeva.A.M и добавляем его в ранее созданную группу.

sudo useradd -U -m -s /bin/bash -G BBMO-01-23 User-Knyazeva.A.M

passwd User-Knyazeva.A.M

![3]()


# Шаг 4
Проверяем наличие пользователя User-Knyazeva.A.M и суперпользователя Super-Knyazeva.A.M в группе group-BBMO-01-23.

groups User-Knyazeva.A.M

groups Super-Knyazeva.A.M

![4]()


# Шаг 5
Наделяем полномочиями пользователя User-Knyazeva.A.M

sudo chmod 770 ~

sudo chown Super-Knyazeva.A.M:BBMO-01-23 ~


# Шаг 6
Проверка механизмов разграничения доступа.

mkdir 1.txt

touch 1.txt

rm 1.txt
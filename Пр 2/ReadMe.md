# Отчет по ПР-2 "Идентификация и аутентификация" ББМО-01-23 Князевой А.М. 


## Шаги выполнения


# Шаг 1


Создаем суперпользователя Super-Knyazeva.A.M
 sudo useradd Super-Knyazeva.A.M
 
 sudo usermod -a -G sudo Super-Knyazeva.A.M
 
 passwd Super-Knyazeva.A.M
 
![1](https://github.com/KnyazevaAM/TOIB/assets/70960325/ca49b542-9f89-4f6e-8a6f-635156154ff2)

![2](https://github.com/KnyazevaAM/TOIB/assets/70960325/09b09da5-423f-471b-8041-51912eb79201)


# Шаг 2

Создаем группу group-BBMO-01-23.

sudo groupadd BBMO-01-23

sudo usermod -aG BBMO-01-23 Super-Knyazeva.A.M


![3](https://github.com/KnyazevaAM/TOIB/assets/70960325/c3a5ecb8-0cd8-46c4-83b1-b56706e9b3a1)



# Шаг 3

Создаем обычного пользователя User-Knyazeva.A.M и добавляем его в ранее созданную группу.

sudo useradd -U -m -s /bin/bash -G BBMO-01-23 User-Knyazeva.A.M

passwd User-Knyazeva.A.M


![4](https://github.com/KnyazevaAM/TOIB/assets/70960325/47be924f-0b7b-4501-b7ad-bf4ebdb034b8)


# Шаг 4
Проверяем наличие пользователя User-Knyazeva.A.M и суперпользователя Super-Knyazeva.A.M в группе group-BBMO-01-23.

groups User-Knyazeva.A.M

groups Super-Knyazeva.A.M


![5](https://github.com/KnyazevaAM/TOIB/assets/70960325/cfc00b20-02c7-4b3d-9e10-ef206e266220)


# Шаг 5
Наделяем полномочиями пользователя User-Knyazeva.A.M

sudo chmod 770 ~

sudo chown Super-Knyazeva.A.M:BBMO-01-23 ~


# Шаг 6
Проверка механизмов разграничения доступа.

mkdir 1.txt

touch 1.txt

rm 1.txt

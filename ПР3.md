# TOIB3


## Создаем 2 виртуальные машины на базе Ubuntu (Ссылка - https://ubuntu.com/download/desktop) и обеспечиваем между ними сетевой обмен.
![image](https://github.com/Flameitser/TOIB3/assets/65831927/c36e9707-850f-4514-984b-bbbb0cc79fe6)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/ba490a6c-f5da-4747-96b9-fdc8a9865f2f)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/577d38cd-b24a-4ac4-944b-b5082a0a7cb9)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/f26318a7-656d-4271-9346-221edc1a1627)

## Устанавливаем, включаем правила TCP и UDP соединения и настраиваем правила rsyslog на сервере и клиенте

**Установка и насйтрока на сервере**

![image](https://github.com/Flameitser/TOIB3/assets/65831927/201397db-a4c0-454d-bddd-cc7996421165)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/9922c21f-ff26-4232-a809-550a001d1d15)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/d18adda7-e7df-4210-8404-ba94183d105c)

**Установка и настройка на клиенте**

![image](https://github.com/Flameitser/TOIB3/assets/65831927/c1ebb168-a2f4-4204-a7b4-56d9502e95ca)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/6bb9a71d-330e-4681-9a4f-72fd738779aa)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/3555ad27-bab7-488c-a5b4-643bb7ae5800)


## Проверяем получения логов на сервере

![image](https://github.com/Flameitser/TOIB3/assets/65831927/3cca438d-7b11-448e-8908-d4158d5441f8)


## Устанавливаем и настраиваем получение логов на сервере с использованием Loki (Предварительно установив docker-compose)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/8352b499-09bf-47a2-a1a7-30368ceca2b5)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/e3e64e65-ead0-41d0-94e0-22359901a0d4)

## Редактируем promtail и docker-compose на клиенте

![image](https://github.com/Flameitser/TOIB3/assets/65831927/9309a639-122b-42c2-b2aa-c8c2e429366d)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/80dbbc9e-b5ba-43eb-b50a-d98ba365e529)


## Просматриваем логи клиента в Grafana

![image](https://github.com/Flameitser/TOIB3/assets/65831927/17de913d-ee64-4aaa-8528-4e98874888a6)


## Установка получения логов на сервере с использованием Signoz
**Установка Signoz выполнена согласно инструкции с сайта: https://signoz.io/docs/install/docker/#install-signoz-using-docker-compose**

![image](https://github.com/Flameitser/TOIB3/assets/65831927/e4ce06ec-db12-4a43-85ba-47728e68712d)

## Установка и настройка sample-nodejs-app на клиенте 
**Установка sample-nodejs-app выполнена согласно инструкции с сайта https://github.com/SigNoz/sample-nodejs-app**
![image](https://github.com/Flameitser/TOIB3/assets/65831927/4f052221-5fde-4029-b78d-09e07d0b68d3)

![image](https://github.com/Flameitser/TOIB3/assets/65831927/6c155647-9717-4f1b-bea7-6406243b19f8)


## Проверка получения логов в Signoz
![image](https://github.com/Flameitser/TOIB3/assets/65831927/17f376be-6ad5-4862-b5e2-dd4e918bcb22)

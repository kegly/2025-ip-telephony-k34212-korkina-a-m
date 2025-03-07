
University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [IP-telephony](https://itmo-ict-faculty.github.io/ip-telephony/)  
Year: 2023/2024  
Group: K34212  
Author: Korkina Anna Mikhailovna
Lab: Lab1  
Date of create: 20.02.2025  
Date of finished: 7.03.2024  


## Отчет по лабораторной работе №1
### ["Базовая настройка ip-телефонов в среде Сisco packet tracer"](https://itmo-ict-faculty.github.io/ip-telephony/education/labs2023_2024/lab1/lab1/)

#### 1. Цель  
Изучить рабочую среду Cisco Packet Tracer, ознакомить- ся с интерфейсами основных устройств, типами кабелей, научиться собирать топологию. Изучить построение сети IP-телефонии с помощью маршрутизатора, коммутатора и IP телефонов Cisco 7960 в среде Packet tracer

#### 2. Задачи Части 1

1. Изучить теоретическую и практическую части лабораторной работы.
2. Собрать схему соединения.
3. Научиться настраивать коммутаторы и компьютеры для полноценной работы сети.
4. Научиться применять основной список команд для конфигурирования устройств сети.
5. После выполнения необходимых настроек необходимо убедиться в том, что любой компьютер одной сети посредством пинга передает пакеты любому компьютеру другой сети.

#### 3. Задачи Части 2

1. Собрать схему соединения, указанную на рисунке
2. Изменить имя маршрутизатора на CMERouter.
3. Настроить интерфейс fa0/0 на маршрутизаторе Cisco 2811 (CMERouter).
4. Настроить DHCP сервера для передачи голоса и данных на маршрутизаторе - Cisco 2811.
5. Настроить услуги телефонии Cisco CallManager Express на маршрутизаторе 2811.
6. Настроить маршрутизацию сети.
7. Создать VLAN порты на коммутаторе для взаимодействия коммутатора с маршрутизатором и подключить IP телефоны.
8. Настроить IP-телефоны, присвоить им номера и соединить с коммутатором.
9. Проверить звонки между телефонами и проверить остальные сервисы (перевод звонков, конференц-связь, перехват звонка).

#### 4. Ход работы  

#### 4.1. Часть 1

Схема соединения.
Добавление роутера так как в задании упоминаютя "разные" сети

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/topology.png)

Настройка роутера - подинтерфейсы 

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/router.png)

Настройка коммутатора - vlan 2, vlan 3 

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/com.png)

Настройка компьютеров - статические ip

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/pc.png)

Проверка соединения между сетями- ping

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/ping.png)


#### 4.2. Часть 2


Схема соединения

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/ip-topol.png)


Настройка роутера - dhcp,  опция 150 для TFTP 

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/ip-dhcp.png)


Настройка роутера - telephone service : IP-адрес голосового шлюза,  автоматическое назначение внешних номеров
Присвоение телефонных номеров нашим 

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/ip-tel.png)


Настройка коммутатора - поддержка Voip

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/ip-com.png)


Проверка звонка

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-1/images/ip-ring.png)




University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [PIN](https://fict.itmo.ru)  
Course: [IP-telephony](https://itmo-ict-faculty.github.io/ip-telephony/)  
Year: 2023/2024  
Group: K34212  
Author: Korkina Anna Kikhailovna
Lab: Lab2  
Date of create: 13.03.2025  
Date of finished: 21.03.2025  
## Отчет по лабораторной работе №2
### ["Конфигурация voip в среде Сisco packet tracer"](https://itmo-ict-faculty.github.io/ip-telephony/education/labs2023_2024/lab2/lab2/)

#### 1. Цель  
Иизучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

#### 2. Задачи Части 1

1. В конфигурационном режиме измените название маршру- тизатора на CMERouter.
2. Отключите синтаксис ввода слов от DNS серверов.
3. Задайте пароли для защиты маршрутизатора как в удаленном режиме, так и в режиме консоли.
4. Настройте интерфейс fa0/0 на маршрутизаторе Cisco 2811 (CMERouter).
5. Настроить DHCP сервера для передачи голоса и данных на маршрутизаторе Cisco 2811.
6. Настроить услуги телефонии Cisco CallManager Express на маршрутизаторе 2811.
7. Создать VLAN порты на коммутаторе Cisco Catalyst 3560 для взаимодействия коммутатора с маршрутизатором и подключить IP телефоны.
8. Настроить IP-телефоны и соединить с коммутатором Cisco Catalyst 3560.
9. Проверить звонки между телефонами и проверить остальные сервисы (перевод звонков, конференц-связь, перехват звонка).

#### 3. Задачи Части 2

1. Создать VLAN порты на коммутаторе для взаимо- действия коммутатора с маршрутизатором и подключить IP телефоны.
2. Задайте маршрут по умолчанию командой ip default-gateway.
3. Настройте порт как канал типа trunk.
4. Настроить DHCP сервера для передачи голоса и данных на маршрутизаторе Cisco 2811.
5. Настроить услуги телефонии Cisco CallManager Express на маршрутизаторе.
6. Настроить IP-телефоны и соединить с коммутатором.
7. Подключить конечные узлы устройств.
8. Проверить звонки между телефонами и проверить остальные сервисы (перевод звонков, конференц-связь, перехват звонка).

#### 4. Ход работы  

#### 4.1. Часть 1

Создана схема cогласно схеме

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/topology.png)

Переименован роутер, отключен синтаксис ввода слов от DNS серверов, заданы пароли

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/tree/main/lab-2/images/no%20domain.png)

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/pass.png)

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/pass-check.png)

Настроен FastEthernet 0/0  + DHCP сервер 

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/tree/main/lab-2/images/ip+dhcp.png)

Услуги телефонии Cisco CallManager Express 

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/tel-ser.png)

Проверка

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/ring.png)

#### 4.2. Часть 2
Новая топология 
![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/tree/main/lab-2/images/top-2.png)
Настройка vlan(100, 200) и интерфейсов 
![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/tree/main/lab-2/images/add-vlan.png)

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/tree/main/lab-2/images/switch-vlan.png)

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/tree/main/lab-2/images/subint.png)

default gateway

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/defget.png)

Проверка

ip из DHCP pool:

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/Screenshot%20from%202025-03-21%2011-16-15.png)

Звонок

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab-2/images/ring2.png)


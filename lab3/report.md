University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [PIN](https://fict.itmo.ru)  
Course: [IP-telephony](https://itmo-ict-faculty.github.io/ip-telephony/)  
Year: 2025  
Group: K34212  
Author: Korkina Anna Mikhailovna
Lab: Lab3  
Date of create: 15.03.2025  
Date of finished: 28.03.2025  


## Отчет по лабораторной работе №3
### ["Использование Asterisk в качестве SIP proxy"](https://itmo-ict-faculty.github.io/ip-telephony/education/labs2023_2024/lab2/lab2/)

#### 1. Цель  

Изучить программный комплекс Asterisk. Настройка Asterisk для локальных звонков.

#### 2. Задачи

1. Установить систему server.
2. Установить Asterisk.
3. Установить soft телефон на рабочую станцию.
4. Настроить SIP каналы.
5. Подключиться к SIP каналам soft телефона.
6. Сделать тестовый звонок на номер 1000


#### 4. Ход работы  

### 4.1 настройка sip в asterisk
Настраиваем согласно документации asterisk


/etc/asterisk/sip.conf

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab3/images/Screenshot%20from%202025-03-28%2012-54-42.png)

 /etc/asterisk/extensions.conf


![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab3/images/Screenshot%20from%202025-03-28%2013-02-00.png)

/etc/asterisk/pjsip.conf

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab3/images/Screenshot%20from%202025-03-28%2013-02-37.png)

Результат
![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab3/images/Screenshot%20from%202025-03-28%2013-08-47.png)

### 4.2 настройка sip account в zoiper

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab3/images/Screenshot%20from%202025-03-28%2013-09-55.png)

звонок 

![image](https://github.com/kegly/2025-ip-telephony-k34212-korkina-a-m/blob/main/lab3/images/Screenshot%20from%202025-03-28%2012-50-36.png)



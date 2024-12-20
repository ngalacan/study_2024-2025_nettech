---
## Front matter
lang: ru-RU
title: Презентация по лабораторной работе №6
subtitle: "Адресация IPv4 и IPv6. Двойной стек"
author:
  - Галацан Николай
institute:
  - Российский университет дружбы народов, Москва, Россия

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---


## Докладчик

  * Галацан Николай
  * 1032225763
  * уч. группа: НПИбд-01-22
  * Факультет физико-математических и естественных наук
  * Российский университет дружбы народов

## Цели и задачи

Изучение принципов распределения и настройки адресного пространства на
устройствах сети.


#  Разбиение сети на подсети

## Выполнение лабораторной работы

| **Характеристика**          | **Значение**                         |
|-----------------------------|--------------------------------------|
| Адрес сети                  | 172.16.20.0/24                       |
| Префикс маски               | /24                                  |
| Маска                       | 255.255.255.0                        |
| Broadcast-адрес             | 172.16.20.255                        |
| Адрес сети в двоичной форме | 10101100.00010000.00010100.00000000  |
| Маска в двоичной форме      | 11111111.1111111.1111111.00000000    |
| Число возможных подсетей    | 2^8=256                              |
| Диапазон адресов узлов      | 172.16.20.1 - 172.16.20.254        |

## Выполнение лабораторной работы

| **Характеристика**          | **Значение**                        |
|-----------------------------|--------------------------------------|
| Адрес сети                  | 10.10.1.64/26                        |
| Префикс маски               | /26                                  |
| Маска                       | 255.255.255.192                      |
| Broadcast-адрес             | 10.10.1.127                          |
| Адрес сети в двоичной форме | 00001010.00001010.00000001.01000000  |
| Маска в двоичной форме      | 11111111.1111111.1111111.11000000    |
| Число возможных подсетей    | 2^6=64                               |
| Диапазон адресов узлов      | 10.10.1.65 - 10.10.1.126             |

## Выполнение лабораторной работы

| **Характеристика**          | **Значение**                         |
|-----------------------------|--------------------------------------|
| Адрес сети                  | 10.10.1.0/26                         |
| Префикс маски               | /26                                  |
| Маска                       | 255.255.255.192                      |
| Broadcast-адрес             | 10.10.1.63                           |
| Адрес сети в двоичной форме | 00001010.00001010.00000001.00000000  |
| Маска в двоичной форме      | 11111111.1111111.1111111.11000000    |
| Число возможных подсетей    | 2^6=64                               |
| Диапазон адресов узлов      | 10.10.1.1 - 10.10.1.62               |

## Выполнение лабораторной работы

| **Характеристика**     | **Значение**                                                           |
|------------------------|------------------------------------------------------------------------|
| Адрес сети             | 2001:db8:c0de::/48                                                     |
| Длина префикса         | 48                                                                     |
| Префикс                | 2001:db8:c0de::                                                        |
| Маска                  | ffff:ffff:ffff:0:0:0:0:0                                |
| Диапазон адресов узлов | 2001:db8:c0de:0:0:0:0 - 2001:db8:c0de:ffff:ffff:ffff:ffff  |

## Выполнение лабораторной работы

| **Характеристика**     | **Значение**                                                                     |
|------------------------|-----------------------------------------------------------------------------------|
| Адрес сети             | 2a02:6b8::/64                                                                     |
| Длина префикса         | 64                                                                                |
| Префикс                | 2a02:6b8:0000:0000                                                                |
| Маска                  | ffff:fffff:ffff:ffff:0:0:0:0                                          |
| Диапазон адресов узлов | 2a02:6b8:: - 2a02:6b8:0:0:ffff:ffff:ffff:ffff   |


# Настройка двойного стека адресации IPv4 и IPv6 в локальной сети

## Выполнение лабораторной работы

![Топология сети с двумя локальными подсетями в GNS3](image/1.png){#fig:1 width=50%}

## Выполнение лабораторной работы

![Настройка IPv4-адресации на PC-1 и PC-2](image/2.png){#fig:2 width=70%}

## Выполнение лабораторной работы

![Настройка IPv4-адресации на сервере](image/3.png){#fig:3 width=70%}

## Выполнение лабораторной работы

![Настройка IPv4-адресации для интерфейсов маршрутизатора FRR](image/4.png){#fig:4 width=70%}


## Выполнение лабораторной работы

![Проверка конфигурации маршрутизатора FRR](image/5.png){#fig:5 width=70%}

## Выполнение лабораторной работы

![Проверка подключения с PC-1](image/6.png){#fig:6 width=70%}

## Выполнение лабораторной работы

![Проверка подключения с PC-2](image/7.png){#fig:7 width=70%}

## Выполнение лабораторной работы

![Настройка IPv6-адресации на PC-3 и PC-4](image/8.png){#fig:8 width=80%}

## Выполнение лабораторной работы

![Настройка IPv6-адресации на сервере](image/9.png){#fig:9 width=70%}

## Выполнение лабораторной работы

![Настройка IPv6-адресации для интерфейсов маршрутизатора VyOS](image/10.png){#fig:10 width=70%}

## Выполнение лабораторной работы

![Сохранение изменений настроек маршрутизатора VyOS](image/11.png){#fig:11 width=70%}

## Выполнение лабораторной работы

![Просмотр интерфейсов маршрутизатора VyOS](image/12.png){#fig:12 width=70%}

## Выполнение лабораторной работы

![Проверка подключения с PC-3](image/13.png){#fig:13 width=70%}

## Выполнение лабораторной работы

![Проверка подключения с PC-4](image/14.png){#fig:14 width=70%}

## Выполнение лабораторной работы


![Проверка доступности устройств из подсети IPv4 для устройств из подсети IPv6](image/15.png){#fig:15 width=70%}

## Выполнение лабораторной работы

![Проверка доступности устройств из подсети IPv6 для устройств из подсети IPv4](image/16.png){#fig:16 width=70%}

## Выполнение лабораторной работы

![Проверка доступности устройств из обеих подсетей с сервера двойного стека ](image/17.png){#fig:17 width=70%}

## Выполнение лабораторной работы

![Захваченный трафик ARP, ICMP, ICMPv6 в Wireshark](image/18.png){#fig:18 width=50%}



# Задание для самостоятельного выполнения

## Выполнение лабораторной работы

- подсеть 1: **IPv4** `10.10.1.96/27`; длина префикса - 27,  маска подсети: 
`255.255.255.224`, broadcast: `10.10.1.127`, диапазон: `10.10.1.97 - 10.10.1.126`; **IPv6** `2001:DB8:1:1::/64`; длина префикса - 64, диапазон: `2001:db8:1:1:0:0:0:0 - 2001:db8:1:1:ffff:ffff:ffff:ffff`;

- подсеть 2: **IPv4** `10.10.1.16/28`; длина префикса - 28, маска подсети: 
`255.255.255.240`, broadcast: `10.10.1.31`, диапазон адресов: `10.10.1.17 - 10.10.1.30`; **IPv6** `2001:DB8:1:4::/64`; длина префикса - 64, диапазон: `2001:db8:1:4:0:0:0:0 - 2001:db8:1:4:ffff:ffff:ffff:ffff`.

## Выполнение лабораторной работы

![Топология сети с двумя локальными подсетями](image/19.png){#fig:19 width=70%}

## Выполнение лабораторной работы

Таблица адресации:

| **Устройство** | **Интерфейс** | **IPv4**        | **IPv6**              | **Шлюз**              |
|----------------|---------------|-----------------|-----------------------|-----------------------|
| PC-1           | NIC           | 10.10.1.99/27   | 2001:db8:1:1::a/64    | 10.10.1.97 / gw-01    |
| PC-2           | NIC           | 10.10.1.18/28   | 2001:db8:1:4::a/64    | 10.10.1.17 / gw-01    |
| gw-01          | eth0          | 10.10.1.97/27   | 2001:db8:1:1::1/64    |                       |
| gw-01          | eth1          | 10.10.1.17/28   | 2001:db8:1:4::1/64    |                       |

## Выполнение лабораторной работы

![Настройка IPv4- и IPv6-адресации на PC-1](image/20.png){#fig:20 width=70%}

## Выполнение лабораторной работы

![Настройка IPv4- и IPv6-адресации на PC-2](image/21.png){#fig:21 width=70%}

## Выполнение лабораторной работы

```
set interfaces ethernet eth0 address 10.10.1.97/27
set interfaces ethernet eth1 address 10.10.1.17.28
compare
commit
save
```

## Выполнение лабораторной работы

![Настройка IPv6-адресации на маршрутизаторе VyOS](image/22.png){#fig:22 width=70%}

## Выполнение лабораторной работы

![Просмотр интерфейсов на маршрутизаторе VyOS](image/23.png){#fig:23 width=70%}

## Выполнение лабораторной работы 

![Проверка подключения с PC-1 на PC-2 по IPv4 и IPv6](image/24.png){#fig:24 width=70%}

## Выполнение лабораторной работы

![Проверка подключения с PC-2 на PC-1 по IPv4 и IPv6](image/25.png){#fig:25 width=70%}


## Выводы

В результате выполнения работы были изучены принципы распределения и настройки адресного пространства на
устройствах сети.



---
## Front matter
lang: ru-RU
title: Презентация по лабораторной работе №3
subtitle: "Анализ трафика в Wireshark"
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

Изучение посредством Wireshark кадров Ethernet, анализ PDU протоколов
транспортного и прикладного уровней стека TCP/IP.



# MAC-адресация

## Выполнение лабораторной работы

![Команда `ipconfig`](image/1.png){#fig:1 width=50%}

## Выполнение лабораторной работы

![Команда `ipconfig /all`](image/2.png){#fig:2 width=70%}

#  Анализ кадров канального уровня в Wireshark

## Выполнение лабораторной работы

![Запуск захвата трафика](image/3.png){#fig:3 width=70%}

## Выполнение лабораторной работы

![Пинг шлюза по умолчанию](image/4.png){#fig:4 width=70%}

## Выполнение лабораторной работы

![Кадр ICMP - эхо-запрос: информация о длине кадра](image/5.png){#fig:5 width=50%}

## Выполнение лабораторной работы

![Кадр ICMP - эхо-запрос: информация о типе Ethernet и MAC-адресах](image/6.png){#fig:6 width=60%}

## Выполнение лабораторной работы

![Кадр ICMP - эхо-ответ: информация о длине кадра, типе Ethernet, MAC-адресах](image/7.png){#fig:7 width=60%}

## Выполнение лабораторной работы

![Кадр ARP](image/8.png){#fig:8 width=70%}

## Выполнение лабораторной работы

![Пинг `vk.com`: запрос](image/9.png){#fig:9 width=70%}

## Выполнение лабораторной работы

![Пинг `vk.com`: ответ](image/10.png){#fig:10 width=70%}

## Выполнение лабораторной работы

![Кадр ARP - эхо-ответ](image/11.png){#fig:11 width=70%}

# Анализ протоколов транспортного уровня в Wireshark

## Выполнение лабораторной работы

![Кадр http - запрос](image/12.png){#fig:12 width=70%}

## Выполнение лабораторной работы

![Кадр http - ответ](image/13.png){#fig:13 width=70%}

## Выполнение лабораторной работы

![Кадр dns - запрос](image/14.png){#fig:14 width=60%}

## Выполнение лабораторной работы

![Кадр dns - ответ](image/15.png){#fig:15 width=70%}

## Выполнение лабораторной работы

![Кадр quic - ответ](image/16.png){#fig:16 width=70%}


# Анализ handshake протокола TCP в Wireshark

## Выполнение лабораторной работы

![Первая ступень handshake TCP](image/17.png){#fig:17 width=60%}

## Выполнение лабораторной работы

![Вторая ступень handshake TCP](image/18.png){#fig:18 width=60%}

## Выполнение лабораторной работы

![Третья ступень handshake TCP](image/19.png){#fig:19 width=60%}

## Выполнение лабораторной работы

![График потока](image/20.png){#fig:20 width=70%}


## Выводы

В результате выполнения работы были изучены посредством Wireshark кадры Ethernet, произведен анализ PDU протоколов транспортного и прикладного уровней стека TCP/IP.



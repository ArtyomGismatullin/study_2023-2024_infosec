---
## Front matter
lang: ru-RU
title: Лабораторная работа №6
subtitle: Мандатное разграничение прав
author:
  - Гисматуллин А.В.
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
 
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
---

## Цели и задачи

 - Развить навыки администрирования ОС Linux. Получить первое практическое знакомство с технологией SELinux1.
 - Проверить работу SELinx на практике совместно с веб-сервером Apache.

# Процесс выполнения лабораторной работы

## Проверка сервера

![Командная строка. Проверка работоспособности сервера](image/01.png){ #fig:001 width=70%, height=70% }

## Проверка сервера

![Командная строка. Веб-сервер запущен в процессе](image/02.png){ #fig:002 width=70%, height=70% }

## Проверка сервера

![Командная строка. Текущее состояние переключателей](image/03.png){ #fig:003 width=70%, height=70% }

## Статистика о политике

![Командная строка. Статистика о политике](image/04.png){ #fig:004 width=70%, height=70% }

## Информация о файлах

![Командная строка. Информация о директории и файле](image/05.png){ #fig:005 width=70%, height=70% }

## Веб-сервер

![Браузер. Проверка отображения файла](image/06.png){ #fig:006 width=70%, height=70% }

## Изменение контекста

![Командная строка. Изменение контекста файла](image/07.png){ #fig:007 width=70%, height=70% }

## Веб-сервер

![Браузер. Попытка посетить сайт](image/08.png){ #fig:008 width=70%, height=70% }

## log-файлы

![Командная строка. Просмотр ошибок](image/09.png){ #fig:009 width=70%, height=70% }

## Изменения файла

![Командная строка. Изменение конфигурационного файла](image/010.png){ #fig:010 width=70%, height=70% }

## Веб-сервер

![Браузер. Попытка соединения](image/011.png){ #fig:011 width=70%, height=70% }

## Просмотр ошибок

![Командная строка. Просмотр ошибок](image/012.png){ #fig:012 width=70%, height=70% }

## Проверка изменений

![Командная строка. Проверка изменений](image/013.png){ #fig:013 width=70%, height=70% }

## Веб-сервер

![Командная строка. Повторный запуск сервера](image/014.png){ #fig:014 width=70%, height=70% }

## Удаление компонентов

![Командная строка. Удаление](image/015.png){ #fig:015 width=70%, height=70% }

# Выводы по проделанной работе

В ходе выполнения данной лабораторной работы были развиты навыки администрирования ОС Linux, а также проверена работа SELinx на практике совместно с веб-сервером Apache.



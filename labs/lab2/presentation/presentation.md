---
## Front matter
lang: ru-RU
title: Лабораторная работа №2
subtitle: Дискреционное разграничение прав Linux
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

- Получение практических навыков работы в консоли с атрибутами файлов
- Закрепление теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux

# Процесс выполнения лабораторной работы

## Создание пользователя и определение его uid и группы

![Командная строка. Работа с пользователем](image/01.png){ #fig:001 width=70%, height=70% }

## Сравнение id и groups

![Командная строка. Сравнение id и groups](image/02.png){ #fig:002 width=70%, height=70% }

## Файл /etc/passwd

![Командная строка. Просмотр файла /etc/passwd](image/03.png){ #fig:003 width=70%, height=70% }

## Команды ls -a

![Командная строка. Команды lsattr и ls -l](image/04.png){ #fig:004 width=70%, height=70% }

## Снятие дистрибутов

![Командная строка. Снятие дистрибутов для dirl](image/05.png){ #fig:005 width=70%, height=70% }

## Права на директорию и файл

![Права на директорию и файл](image/06.png){ #fig:006 width=70%, height=70% }

# Выводы по проделанной работе

В ходе выполнения данной лабораторной работы были получены практические навыки работы в консоли с атрибутами файлов, закреплены теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux1.



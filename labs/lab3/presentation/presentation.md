---
## Front matter
lang: ru-RU
title: Лабораторная работа №3
subtitle: Дискреционное разграничение прав Linux для групп пользователей
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

- Получение практических навыков работы в консоли с атрибутами файлов для групп пользователей

# Процесс выполнения лабораторной работы

## Создание пользователя guest2 и определение его в группы

![Командная строка. Работа с пользователем guest2](image/01.png){ #fig:001 width=70%, height=70% }

## Работа с пользователями guest и guest2

![Командная строка. Работа с пользователями](image/02.png){ #fig:002 width=70%, height=70% }

## Файл /etc/group

![Командная строка. Команда cat /etc/group](image/03.png){ #fig:003 width=70%, height=70% }

## Изменение прав доступа

![Командная строка. Изменение прав доступа](image/04.png){ #fig:004 width=70%, height=70% }

## Для пользователя guest2

![Командная строка. Изменение прав доступа 2](image/05.png){ #fig:005 width=70%, height=70% }

## Права на директорию и файл

![Права на директорию и файл](image/06.png){ #fig:006 width=70%, height=70% }

# Выводы по проделанной работе

В ходе выполнения данной лабораторной работы были получены практические навыки работы в консоли с атрибутами файлов для групп пользователей



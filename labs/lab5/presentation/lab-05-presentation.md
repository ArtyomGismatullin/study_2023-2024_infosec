---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
subtitle: Дискреционное разграничение прав Linux. Исследования влияния расширенных атрибутов
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

 - Изучение механизмов изменения идентификаторов, применения SetUID- и Sticky-битов. 
 - Получение практических навыков работы в консоли с дополнительными атрибутами. 
 - Рассмотрение работы механизма смены идентификатора процессов пользователей,
 а также влияние бита Sticky на запись и удаление файлов

# Процесс выполнения лабораторной работы

## Файл simpleid.c

![Редактор. Файл simpleid.c](image/01.png){ #fig:001 width=70%, height=70% }

## Сравнение с системной командой

![Командная строка. Сравнение с выводом id](image/02.png){ #fig:002 width=70%, height=70% }

## Simpleid2.c

![Редактор. Новая программа](image/03.png){ #fig:003 width=70%, height=70% }

## Изменение владельца и атрибутов

![Командная строка. Изменение владельца и атрибутов файла](image/04.png){ #fig:004 width=70%, height=70% }

## Сравнение вывода

![Командная строка. Сравнение результатов вывода](image/05.png){ #fig:005 width=70%, height=70% }

## Readfile

![Редактор. Файл readfile](image/06.png){ #fig:006 width=70%, height=70% }

## SetU'D-бит

![Командная строка. Проверка изменений](image/07.png){ #fig:007 width=70%, height=70% }

## Исследование Stiky-бита

![Командная строка. Исследование Stiky-бита](image/08.png){ #fig:008 width=70%, height=70% }

## Исследование Stiky-бита

![Командная строка. Исследование Stiky-бита](image/09.png){ #fig:009 width=70%, height=70% }

# Выводы по проделанной работе

В ходе выполнения данной лабораторной работы были изучены механизмы изменения идентификаторов, применения SetUID- и Sticky-битов. 
Получены практические навыки работы в консоли с дополнительными атрибутами. 
Рассмотрены работы механизма смены идентификатора процессов пользователей,
 а также влияние бита Sticky на запись и удаление файлов



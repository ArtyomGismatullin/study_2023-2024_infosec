---
## Front matter
lang: ru-RU
title: Лабораторная работа №4
subtitle: Дискреционное разграничение прав Linux. Расширенные атрибуты
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

## Проверка атрибутов файла

![Командная строка. Попытка изменения расширенных атрибутов](image/01.png){ #fig:002 width=70%, height=70% }

## Команда chattr

![Командная строка. Команда chattr +a](image/02.png){ #fig:003 width=70%, height=70% }

## Изменение атрибута а

![Командная строка. После изменения расширенных атрибутов](image/03.png){ #fig:004 width=70%, height=70% }

## Возврат изменений

![Командная строка. Последствия возврата атрибутов](image/04.png){ #fig:005 width=70%, height=70% }

## Атрибут i

![Командная строка. Изменение атрибута i](image/05.png){ #fig:006 width=70%, height=70% }

## Права на директорию и файл

![Командная строка. При атрибуте i](image/06.png){ #fig:007 width=70%, height=70% }

# Выводы по проделанной работе

В ходе выполнения данной лабораторной работы были получены практические навыки работы в консоли с расширенными атрибутами файлов



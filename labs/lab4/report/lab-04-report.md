---
## Front matter
title: "Отчет по лабораторной работе №4"
subtitle: "Дискреционное разграничение прав Linux. Расширенные атрибуты"
author: "Гисматуллин Артём Вадимович НПИбд-01-22"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Получение практических навыков работы в консоли с расширенными атрибутами файлов

# Задание

Последовательно выполнять все пункты, занося ответы и замечания в отчет.

# Выполнение лабораторной работы

1. Зайдем под учетной записью guest и проверим расширенные атрибуты файла file1 командой lsattr (рис. [-@fig:001])

![Командная строка. Проверка расширенных атрибутов файла file1](image/01.png){ #fig:001 width=70%, height=70% }

2. После этого дадим владельцу файла права на чтение и запись файла, а также попытаемся изменить расширенные атрибуты файла. Операция выполнена неуспешно (рис. [-@fig:002])

![Командная строка. Попытка изменения расширенных атрибутов](image/01.png){ #fig:002 width=70%, height=70% }

3. Для изменения расширенных атрибутов (атрибута a) зайдем под учетной записью root и пропишем ту же команду chattr +a (рис. [-@fig:003])

![Командная строка. Команда chattr +a](image/02.png){ #fig:003 width=70%, height=70% }

4. Далее производим попытки записать что-то в файл (успешно), перезаписать его, а также переименовать/удалить (неуспешно) (рис. [-@fig:004])

![Командная строка. После изменения расширенных атрибутов](image/03.png){ #fig:004 width=70%, height=70% }

Неуспешные попытки связаны с тем, что расширенный атрибут a дает возможность лишь дописывать что-то в файл (рис. [-@fig:005])

![Командная строка. Последствия возврата атрибутов](image/04.png){ #fig:005 width=70%, height=70% }

Как видим, теперь все работает успешно. Но изменения будут иные, если мы изменим уже атрибут i (рис. [-@fig:006])

![Командная строка. Изменение атрибута i](image/05.png){ #fig:006 width=70%, height=70% }

5. Теперь попробуем выполнить те же команды (рис. [-@fig:007])

![Командная строка. При атрибуте i](image/06.png){ #fig:007 width=70%, height=70% }

Как можем увидеть, атрибут i запрещает изменения, удаления и переименование файла

# Выводы

В ходе выполнения данной лабораторной работы были получены практические навыки работы в консоли с расширенными атрибутами файлов

# Список литературы{.unnumbered}

1. [Теория разграничения прав пользователей](https://moodle.kstu.ru/pluginfile.php/318215/mod_resource/content/1/Теория_разграничение_прав_пользователи.pdf)
2. [Разрешения доступа к файлам](https://linuxcommand.ru/razresheniya-dostupa-k-failam/)

---
## Front matter
title: "Отчет 4 этапу индивидуального проекта"
subtitle: "Использование Nikto"
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

Получение практических навыков работы с Nikto и нахождению уязвимостей.

# Задание

Последовательно выполнять все пункты, занося ответы и замечания в отчет.

# Выполнение лабораторной работы

1. Первым делом получим справочную информацию по сканеру безопасности Nikto командой nikto -h (рис. [-@fig:001])

![Просмотр справочной информации](image/01.png){ #fig:001 width=70%, height=70% }

2. После этого попробуем найти уязвимости сайта gazel.me, где обнаружится 20 уязвимостей (рис. [-@fig:002])

![Проверка gazel.me](image/02.png){ #fig:002 width=70%, height=70% }

3. Затем запустим свой веб-сервис командой service apache2 start, как в предыдущей стадии и попробуем найти уязвимости здесь (не обнаружено) (метод GET) (рис. [-@fig:003])

![Поиск уязвимостей на локальном сервере](image/03.png){ #fig:003 width=70%, height=70% }

4. Далее испытаем ранее установленную DVWA и проанализируем на предмет уязвимостей командой nikto -h http://127.0.0.1/DVWA/ (Уязвимостей снова не было обнаружено) (рис. [-@fig:004])

![Проверка DVWA](image/04.png){ #fig:004 width=70%, height=70% }


# Выводы

В ходе выполнения данного этапа были получены практические навыки работы с Nikto и поиском уязвимостей


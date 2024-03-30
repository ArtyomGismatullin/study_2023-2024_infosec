---
## Front matter
title: "Отчет 3 этапу индивидуального проекта"
subtitle: "Использование Hydra"
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

Получение практических навыков работы с Hydra и подбором паролей.

# Задание

Последовательно выполнять все пункты, занося ответы и замечания в отчет.

# Выполнение лабораторной работы

1.Первым делом перейдем в раздел DVWA Security и поставим низкий уровень безопасности (рис. [-@fig:001])

![Установка низкого уровня безопасности](image/01.png){ #fig:001 width=70%, height=70% }

2. После этого создадим файл password.txt, куда поместим примерные "простые" пароли, которые могут подойти к аккаунту пользователя-жертвы атаки (рис. [-@fig:002])

![Заполнение файла с паролями](image/02.png){ #fig:002 width=70%, height=70% }

3. Открываем затем на сайте Brute Force раздел и попытаемся подобрать имя и пароль пользователя. После неудачной попытки откроем исходный код страницы и проверим метод отправки данных формы (метод GET) (рис. [-@fig:003])

![Поиск метода отправки данных](image/03.png){ #fig:003 width=70%, height=70% }

4. Далее для формирования запроса к Hydra нам потребуется информация о PHPSEESID. Для этого во вкладке Inspect страницы найдем в Storage графу об этом (рис. [-@fig:004])

![PHPSEESID](image/04.png){ #fig:004 width=70%, height=70% }

Так как у нас есть все для отправки запроса, формируем его на основе теоретических данных проекта (рис. [-@fig:005])

![Формирование запроса к Hydra](image/05.png){ #fig:005 width=70%, height=70% }

Как видим, нам подошли логин admin и пароль password. Попробуем войти под этой учетной записью (рис. [-@fig:006])

![Проверка данных](image/06.png){ #fig:006 width=70%, height=70% }

Успех!

# Выводы

В ходе выполнения данного этапа были получены практические навыки работы с Hydra и подбора паролей.


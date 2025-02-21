---
## Front matter
title: "Индивидуальный проект. Этап 1"
subtitle: "Основы информационной безопасности"
author: "Жибицкая Евгения Дмитриевна"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Установка и настройка ОС Kali linux на виртуальную машину.

# Выполнение лабораторной работы

Заранее установим образ диска с официального сайта kali (рис. [-@fig:001]).

![Скачивания iso](image/1.jpg){#fig:001 width=70%}

Затем перейдем в Virtual box, создадим там машину, указав все необходимые параметры - имя, выделенную память, процессоры и тд(рис. [-@fig:002]).

![Создание виртуальной машины](image/2.jpg){#fig:002 width=70%}

Переходим к установке. Указываем местоположение, язык, имя пользователя, место установки и остальные параметры(рис. [-@fig:003]) и (рис. [-@fig:004]).

![Установка ОС](image/3.jpg){#fig:003 width=70%}


![Создание пользователя](image/4.jpg){#fig:004 width=70%}


По завершении установки, перезапускаем и входим в систему(рис. [-@fig:005]).

![Запуск ОС Kali](image/5.jpg){#fig:005 width=70%}


# Выводы

В ходе работы были приобретены навыки по созданию виртуальной машины, установлена и налажена ОС Kali.

# Список литературы{.unnumbered}

[Установка ОС](https://www.kali.org/)


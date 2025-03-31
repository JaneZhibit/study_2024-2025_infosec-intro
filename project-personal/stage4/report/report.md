---
## Front matter
title: "Индивидуальный проект. Этап 4"
subtitle: "Дисцилпина: Основы информационной безопасности"
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

Продолжение выполнения проекта. Освоение приложения nikto


# Выполнение лабораторной работы

Запускаем сервер и работу DVWA - включаем mysql и apache2(рис. [-@fig:001]).

![Запуск DVWA](image/1.jpg){#fig:001 width=70%}

Входим в систему, переходим в раздел Security и для удобства устанавливаем уроень low. Это не обязательно, но все  равно сделаем(рис. [-@fig:002]).

![DVWA Security](image/2.jpg){#fig:002 width=70%}


Затем запустим nikto. Получим и изучим справку.

nikto — базовый сканер безопасности веб-сервера. Он сканирует и обнаруживает уязвимости в веб-приложениях, обычно вызванные неправильной конфигурацией на самом сервере, файлами, установленными по умолчанию, и небезопасными файлами, а также устаревшими серверными приложениями.

(рис. [-@fig:003]).

![Справка о nikto](image/3.jpg){#fig:003 width=70%}

Далее перейдем к получению информации и ее анализу. Получим ее двумя разными способами(через адрес и через имя хоста и номер порта)(рис. [-@fig:004]) и рис. [-@fig:005]).

![Анализ через адрес](image/4.jpg){#fig:004 width=70%}

![Анализ по имени хоста и порту](image/5.jpg){#fig:005 width=70%}

# Выводы

В ходе работы мы познакомились с приложением nikto. Также был произведен анализ DVWA, получена информация о нем.

# Список литературы{.unnumbered}

 - Парасрам, Ш. Kali Linux: Тестирование на проникновение и безопасность : Для профессионалов. Kali Linux / Ш. Парасрам, А. Замм, Т. Хериянто, и др. – Санкт-Петербург : Питер, 2022. – 448 сс.

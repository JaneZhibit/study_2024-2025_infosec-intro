---
## Front matter
title: "Лаброаторная работа №4"
subtitle: "Дисциплина: Основы информационной безопасности"
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

Получение навыков работы в консоли с расширенными атрибутами на ОС Linux Rocky.

# Выполнение лабораторной работы

Сменяем сразу пользователя на guest и определяем расширенные атрибуты фалйа file1 и устанавливаем на него права на чтение и запись(рис. [-@fig:001]).

![Атрибуты файла](image/1.jpg){#fig:001 width=70%}

Затем от имени суперпользователя(от guest это сделать невозможно) устанавливаем на тот же файл атрибут +а, проверим, что все установилось уже от пользователя guest(рис. [-@fig:002]) и рис. [-@fig:003]).

![Атрибут +а от администратора](image/2.jpg){#fig:002 width=70%}
.

![Атрибут +a от gguest](image/3.jpg){#fig:003 width=70%}

Произведем дозапись в файл и убедимся в корректности(рис. [-@fig:004]).

![Дозапись в файл](image/4.jpg){#fig:004 width=70%}

Попробуем удалить или стереть информацию, а затем попытаемся  установить права запрещающие чтение и запись для владельца(рис. [-@fig:005).

![Попытка удаления и изменения прав](image/5.jpg){#fig:005 width=70%}

Снимем атрибут а и попробуем выполнить не удавшиеся команды еще раз(рис. [-@fig:006]).

![Снятие атрибута, повторное выполнение команд](image/6.jpg){#fig:006 width=70%}


Затем поставим атрибут +i и проделаем аналогичные действия, чтобы посмотреть какие из них возможно выполнить, а какие нетрис. [-@fig:007]).

![Атрибут +i](image/7.jpg){#fig:007 width=70%}




# Выводы

В ходе работы были повышены навыки использования консоли при работе с атрибутами(основыными и расширенными) при разграничении доступа.

# Список литературы{.unnumbered}


[ТУИС](https://esystem.rudn.ru)




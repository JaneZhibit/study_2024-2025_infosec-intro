---
## Front matter
lang: ru-RU
title: Лабораторная №5
subtitle: Основы информационной безопасности
author:
  - Жибицкая Е.Д.
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
---



# Цель

## Цель работы

- Продолжение работы на ОС Rocky. Изучение механизмов изменения идентификаторов, применения SetUID- и Sticky-битов и рассмотрение работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.

# Ход работы 


## Подготовка к работе

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Проверка gcc](image/1.jpg)

:::
::::::::::::::



## Simpleid.с

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Создание файла simpleid.c](image/2.jpg)

:::
::: {.column width="50%"}

![Запуск файла](image/3.jpg)

:::
::::::::::::::



## Simpleid2.c
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Файл simpleid2.c](image/4.jpg)
:::
::::::::::::::

## Добавление прав и владельца
 
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Работа с правами](image/5.jpg)

:::
::: {.column width="40%"}

![Исполнение simpleid2.c](image/6.jpg)
:::
::::::::::::::

## Readfile

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

Создадим файл, предназначенный для считывния файлов, вставим код и скомпилируем его
:::
::: {.column width="50%"}

![Файл readfile](image/7.jpg)
:::
::::::::::::::


## Запуск Readfile


:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Работа с правами](image/8.jpg)
:::
::: {.column width="50%"}

![Запуск](image/9.jpg)
:::
::::::::::::::

## Sticky-bit
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

 Сначала проверем установлен ли на директорию stiky-бит, запишем в него сообщение. Посмотрим на установленные права, разрешим чтение и запись для всех остальных пользователей.
:::
::: {.column width="50%"}

![Sticky-бит](image/10.jpg)
:::
::::::::::::::

## Выполнение команд от guest2
:::::::::::::: {.columns align=center}
::: {.column width="50%"}


![Чтение от guest2](image/11.jpg){#fig:011 width=70%}
:::
::: {.column width="50%"}
От пользователя guest2 прочитаем файл, попробуем записать туда текст(безуспешно)Попробуем удалить файл - также безуспешно.
:::
::::::::::::::

## Удаление sticky-bit
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Удаление  файла без sticky-бита](image/13.jpg)
:::
::::::::::::::

## Возвращение sticky-bit
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Возвращение sticky-бита](image/14.jpg)
:::
::::::::::::::

# Выводы

## Вывод

-  В ходе работы были изучены механизмы изменения идентификаторов, применения
SetUID- и Sticky-битов а также влияние бита Sticky на запись и удаление файлов.


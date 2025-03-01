---
## Front matter
lang: ru-RU
title: Индивидуальный проект. Этап 2
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

- Работа с ОС Kali Linux, установка на нее и подготовка к работе DVWA 

# Ход работы 


## Клонирование репозитория

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Клонирование репозитория](image/1.jpg)

:::
::: {.column width="40%"}

Переходим по ссылке  https://github.com/digininja/DVWA в нужный репозиторий, открываем терминал и скачиваем его. Затем перемещаем в каталог /var/www/html. Также повышаем права до максимального уровня

:::
::::::::::::::



## Настройка mysql

:::::::::::::: {.columns align=center}
::: {.column width="50%"}


![Запуск mysql](image/2.jpg)

:::
::: {.column width="50%"}

![Файл config.inc.php](image/3.jpg)
:::
::::::::::::::



## MariaDB
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

MariaDB [(none)]> create database dvwa;

MariaDB [(none)]> create user dvwa@localhost identified by 'p@ssw0rd';

MariaDB [(none)]> grant all on dvwa.* to dvwa@localhost;


MariaDB [(none)]> flush privileges;
:::
::: {.column width="50%"}

![Настройки MAriaDB](image/4.jpg)
:::
::::::::::::::

## Apache2
 
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Запуск apache2](image/5.jpg)

:::
::: {.column width="40%"}

![Редактирование pph.ini](image/6.jpg)

:::
::::::::::::::

## Хост

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![127.0.0.1/DVWA/setup.php](image/7.jpg)

:::
::: {.column width="50%"}

![Вход в систему](image/8.jpg)
:::
::::::::::::::


## Установка завершена

:::::::::::::: {.columns align=center}
::: {.column width="50%"}


![Домашняя страница](image/9.jpg)
:::

::::::::::::::

# Выводы

## Вывод

- В ходе работы была установлена DVWA в гостевую систему Kali Linux, создана ДБ и произведена настройка



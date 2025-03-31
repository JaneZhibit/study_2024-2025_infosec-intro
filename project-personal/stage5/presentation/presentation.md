---
## Front matter
lang: ru-RU
title: Индивидуальный проект. Этап 5
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

 - Завершение выполнения индивидуального проекта. Знакомство и освоение Burp Suite

# Ход работы 


## Подготовка к работе
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Запуск mysql и apache2](image/1.jpg)

:::
::: {.column width="50%"}

![Запуск burpsuite](image/2.jpg)
:::
::::::::::::::



## Настройка
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Настройки соединения](image/3.jpg)
:::
::: {.column width="40%"}

![Параметр network.proxy.allow_hijacking_localhost](image/6.jpg)
:::
::::::::::::::

## Настройка внутри приложения

:::::::::::::: {.columns align=center}
::: {.column width="45%"}

![Настройки приложения](image/4.jpg)

:::
::: {.column width="50%"}

![Включение intercept](image/5.jpg)
:::
::::::::::::::

## Получение запросов

:::::::::::::: {.columns align=center}
::: {.column width="45%"}

Заходим на DVWA и смотрим, что появляется во вкладке Proxy


:::
::: {.column width="50%"}

![Переход на DVWA](image/7.jpg)
:::
::::::::::::::

## Авторизация

:::::::::::::: {.columns align=center}
::: {.column width="45%"}

![Запросы](image/8.jpg)
:::
::: {.column width="50%"}

![Попытка авторизации](image/9.jpg)
:::
::::::::::::::

## Intruder

:::::::::::::: {.columns align=center}
::: {.column width="45%"}
![Перенаправление в Intruder](image/10.jpg)
:::
::::::::::::::

## Cluster bomb attack

:::::::::::::: {.columns align=center}
::: {.column width="45%"}

![Cluster bomb attack](image/11.jpg)
:::
::: {.column width="40%"}

![Заполнение данных](image/12.jpg)

:::
::::::::::::::

## Результаты атаки

:::::::::::::: {.columns align=center}
::: {.column width="60%"}

![Атака](image/13.jpg)
:::
::: {.column width="35%"}

![Успешный подбор](image/14.jpg)

:::
::::::::::::::

## Repeater

:::::::::::::: {.columns align=center}
::: {.column width="45%"}


![Reapeter](image/15.jpg)
:::
::: {.column width="50%"}

Изучим также работы repeater. Перенаправим туда любой результат, посмотрим на его ответ в виде render - увидим страницу входа.

:::
::::::::::::::


# Выводы

## Вывод

- В ходе работы было произведена знакомство с Burp Suite, произведен анализ работы и  принцип атаки подбора данных для входа



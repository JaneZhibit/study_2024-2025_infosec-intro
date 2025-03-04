---
## Front matter
lang: ru-RU
title: Лабораторная №4
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

- Получение навыков работы в консоли с расширенными атрибутами на ОС Linux Rocky

# Ход работы 


## Просмотр атрибутов файла

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

Сменяем сразу пользователя на guest и определяем расширенные атрибуты фалйа file1 и устанавливаем на него права на чтение и запись.

:::
::: {.column width="40%"}

![Атрибуты файла](image/1.jpg)

:::
::::::::::::::



## Добавление +a

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Атрибут +а от администратора](image/2.jpg)

:::
::: {.column width="50%"}

![Атрибут +a от guest](image/3.jpg)
:::
::::::::::::::

## Работа с файлом
 
:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Дозапись в файл](image/4.jpg)
:::
::: {.column width="40%"}

![Попытка удаления и изменения прав](image/5.jpg)

:::
::::::::::::::

## Снятие атрибута

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

![Снятие атрибута, повторное выполнение команд](image/6.jpg)

:::
::::::::::::::


## Атрибут +i

:::::::::::::: {.columns align=center}
::: {.column width="60%"}

![Атрибут +i](image/7.jpg)
:::
::::::::::::::


# Выводы

## Вывод

- В ходе работы были повышены навыки использования консоли при работе с атрибутами(основыными и расширенными) при разграничении доступа




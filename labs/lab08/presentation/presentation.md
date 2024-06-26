---
## Front matter
lang: ru-RU
title: Научная презентация
subtitle: Лабораторная работа №8
author:
  - Выборнов Д. В.
institute:
  - Российский университет дружбы народов, Москва, России
date: 30 марта 2024

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
 - '\makeatletter'
 - '\beamer@ignorenonframetrue'
 - '\makeatother'



---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Выборнов Дмитрий Валерьевич
  * Студент кафедры физико - математических и естесственных наук.
  * Российский университет дружбы народов

:::
::: {.column width="30%"}

:::
::::::::::::::

# Вводная часть

## Актуальность

- Опыт использования инструментов поиска для файлов, фильтрации данных, управления процессами, обслуживания файловых систем и проверке использования диска нужны всем, кто собирается работать с компьютерами.
## Объект и предмет исследования

- Потоки ввода - вывода.
- Команды для поиска и сортировки.
- Команды для обслужимания файловых систем и диска компьютера.

## Цели и задачи

- Изучить принцип работы команд терминала Linux для поиска и сортировки, команд для обслуживания файловых систем и диска компьютера.
- Получить опыт работы с этими командами.

## Материалы и методы

- ОС Linux.
- Редактор gedit.

# Команды

## Специальные потоки

- По умолчанию открыто 3 специальных потока:
- stdin (для входа)
- stoud (для выхода)
- stderr (для ошибок)

## Структуры для сортировки

- Для нахождения конкретных файлов используется find.
- Для нахождения строк в файле используется grep.
- Для сортировки используется sort.

## Конвейеры

- Несколько команд можно соединить в цепочку, поставив между ними |.

## Проверка использования диска

- Для просмотра разделов диска используется df.
- Для просмотра того, сколько памяти занимает конкретный файл, используется du.

## Процессы

- Любую команду можно запустить в фоновом режиме при помощи &.
- Остановить любую задачу можно при помощи команды kill.
- Посмотреть все активные процессы можно при помощи ps.

# Результаты

- Полученный в результате выполнения этой лабораторной работы опыт поможет любому, кто планирует работать с компьютерами.

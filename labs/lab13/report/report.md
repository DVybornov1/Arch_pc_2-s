---
## Front matter
title: "Отчёт по лабораторной работе №13"
subtitle: "НКАбд-02-23"
author: "Выборнов Дмитрий Валерьевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: false # Table of contents
toc-depth: 2
lof: false # List of figures
lot: false # List of tables
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

Изучить основы программирования в оболочке ОС UNIX. Научится писать более
сложные командные файлы с использованием логических управляющих конструкций
и циклов.

# Задание

1. Первое задание.
2. Второе задание.
3. Третье задание.
4. Четвёртое задание.

# Выполнение лабораторной работы

## Первое задание

Я написал программу, которая может найти нужнуй строку в указанном файле. Для этого я использовал команды grep, и ключи inputfile, outputfile, -p -C и -n. После этого я проверил работу этого файла при помощи созданного случайным образом файла.

## Второе задание.

Сначала я создал программу checker на языке C, которая получает число и проверяет, является ли оно больше, меньше или равно нулю. После этого я создал сам командный файл, вызывающий эту программу и переводящий результат её работы в текст. После этого я убедился, что эта программа работает.

## Третье задание

Я создал командный файл, создающий или удаляющий указанное число пронумированных файлов. 

## Четвёртое задание

Я ннаписал командный файл, запаковываущий одну директорию в архив при помощи команды tar. После этого я модифицировал её так, чтобы она запаковывала только файлы, изменённые одну неделю назад.

# Выводы

После выполнения этой лабораторной работы я научился писать более сложные программы в оболочке ОС Linux.

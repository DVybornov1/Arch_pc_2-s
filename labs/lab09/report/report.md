---
## Front matter
title: "Лабораторная работа"
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

Целью этой лабораторной работы является ознакомление и получение опыта работы с командной оболочкой Midnight Commander.

# Задание

- Задания по mc.
- Задания по встроенному редактору mc.
- Ответы на контрольные вопросы.

# Теоретическое введение

Командная оболочка — интерфейс взаимодействия пользователя с операционной системой и программным обеспечением посредством команд.
Midnight Commander (или mc) — псевдографическая командная оболочка для UNIX/Linux
систем.

# Выполнение лабораторной работы

1. Я запускаю mc, создаю несколько файлов для тестирования и на них проверяю работу основных операций и команд меню. После этого я использую один из файлов для проверки возможностей подменю файл, команда и настройки.
2. Я создаю файл text.txt, открываю его и вставляю в него небольшой фрагмент текста, после чего проделываю сним все указанные манипуляции. После этого я открываю файл с исходным кодом C++ и несколько раз включаю и выключаю подсветку синтаксиса.

# Выводы

Выполнив эту лабораторную работу, я получил опыт работы с mc.

# Ответы на контрольные вопросы

1. Всего в mc есть 5 режимов: normal mode, file edit mode, layouts mode, archive view mode и quick image viev mode.
2. Такие команды как, например, chmod, chown, mv или mkdir можно выполнить и при помощи команд, и с помощью комбинаций клавиш.
3. Меню панелей содержит команды для сортировки нахождения и просмотра нужных файлов.
4. Меню файл содержит команды для перемещения и изменения файлов.
5. Меню команда содержит команды для нахождения и просмотра директорий.
6. В меню настройки можно изменить настройки самой командной оболочки.
7. Встроенные команды mc, такие, как help, menu, copy, mkdir и delete используются для создания, перемещения и изменения файлов и директорий.
8. Встроенные команды редактора mc, такие, как cut, paste и undo используются для изменения открытого файла и перемещения по нему.
9. Средства для создания и изменения пользовательских меню содержатся в меню User menu.
10. Для выполнения действий, определяемых пользователем, над некоторым файлом, в mc существует возможность создания пользовательских команд.

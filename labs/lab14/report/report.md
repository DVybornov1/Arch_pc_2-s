---
## Front matter
title: "Отчёт по лабораторной работе №14"
subtitle: "НКАбд-02-24"
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

Целью этой лабораторной работы является получение опыта созданий программ в ОС Linux.

# Выполнение лабораторной работы

1. Я написал командный файл, реализующий упращённый механизм семафоров. Я сделал это при помощи создания и удаления нескольких папок. После этого я проверил работу этой программы в трёх разных терминалах. Также я написал эту программу так, чтобы она удаляла все созданные ей файлы после завершения программы.
2. Я создал программу, которая иммитирует команду man при помощи каталога /usr/share/man/man1. Также программа выдаст особое сообщение, если справки по выбранной команде не существует.
3. Я написал программу, выводящую случайную строку из 10 английских букв при помощи переменной $RANDOM, значение которой делится на количество буков в алфавите.

# Выводы

Выполнив эту лабораторную работу, я получил опыт работы с оболочкой ОС Linux.

# Контрольные вопросы

1. Здесь вместо != должно быть <>.
2. Соединить несколько строк можно либо с помощью join, либо при помощи printf.\
3. Самый простой способ реализовать seq в shell - через цикл for.
4. Получится 3.33.
5. zsh и bash похожи, но zsh имеет больше встроенных команд и более гибкую грамматику этих команд.
6. LIMIT - переменная, следовательно перед ней должен быть $.
7. bash - простая и интуитивная оболочка, по умолчанию имеющаяся во многих операционных системах, но она медленно работает и заниматься отладкой ошибок в ней сложнее, чем в других оболочках. 

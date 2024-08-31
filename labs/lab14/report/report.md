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

Целью этой лабораторной работы является получение опыта созданий программ в shell.

# Выполнение лабораторной работы

2. Я создал программу, которая выводит содержимое файлов man и работает для всех команд, выводя сообщение об ошибке для тех команд, у которых этого файла нет.
3. Я написал программу, выводящую случайную букву, при помощи printf.

# Выводы

Выполнив эту лабораторную работу, я получил опыт работы с shell.

# Контрольные вопросы

1. Здесь вместо != должно быть <>.
2. Соединить несколько строк можно либо с помощью join, либо при помощи printf.\
3. Самый простой способ реализовать seq в shell - через цикл for.
4. Получится 3.33.
5. zsh и bash похожи, но zsh имеет больше встроенных команд и более гибкую грамматику этих команд.
6. LIMIT - переменная, следовательно перед ней должен быть $.
7.ash - простая и интуитивная оболочка, по умолчанию имеющаяся во многих операционных системах, но она медленно работает и заниматься отладкой ошибок в ней сложнее, чем в других оболочках. 

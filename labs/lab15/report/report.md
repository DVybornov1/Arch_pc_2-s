---
## Front matter
title: "Отчёт по Индивидуальному Проекту"
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

Целью этой работы является получение опыта создания вебсайтов и работы с gitpages и Hugo.

# Задание

1. Создать свой собственный сайт.
2. Разместить его на gitpages.
3. Добавить информацию о себе.
4. Сделать несколько постов.
5. Добавить поддержку двух языков.

# Теоретическое введение

Hugo - это быстрый и мощный статический генератор сайтов, написанный на Go. Он позволяет создавать статические веб-сайты, что означает, что HTML-страницы генерируются заранее, а не в режиме реального времени, как в динамических сайтах.

# Реализация проекта

1. Сначала я установил всё необходимое ПО и скачал тему сайта Hugo Academic. Далее создал новый репозиторий git и разместил параметр url для сайта. Далее я изменил некоторые настройки git и разместил новый репозиторий на gitpages.
2. Далее я полностью изменил файл index.md в директории authors/admin, добавив всю нужную информацию о себе. Далее я сделал посты по прошедшей неделе и о Системе управления версиями Git.
3. После этого я сделал посты по темам "Язык разметки Markdown" и "Создание презентаций".
4. Следующим шагом я зарегистрировался на всех указанных сайтах и дабавил ссылки на них в свой сайт. После этого я сделал пост на тему "Языки научного программированияя".
5. В последнюю очередь я добавил своему сайту поддержку двух языков и сделал двуязычный пост по теме "Новые языки программирования".

# Выводы

Выполнив этот индивидуальный проект, я научился создавать вебсайты при помощи Hugo и Gitpages.

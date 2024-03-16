---
## Front matter
title: "Отчёта по лабораторной работе №5"
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
lof: false# List of figures
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

Целью этой лабораторной работы является настройка рабочего стола и получение опыта работы с различным програмным обеспечением.

# Задание

Установка нужного програмного обеспечения и его настройка.

# Выполнение лабораторной работы

1. Сначала я устанавливаю pass и gopass. Потом я генерирую новый ключ gpg создаю новую структуру git. 

2. Так как я работаю с wsl, мне нужно скачать как версию browserpass для Linux, так и расширение для браузера, что я и делаю.

3. Я создаю новый файл для хранения паролей, отображаю пароль для этого имени файла и заменяю существующий пароль на случайный.

4. Я скачиваю дополнительное програмное обеспечение, хотя fonawesome-fonts и iosevka-fonts имеют другие названия и устанавливать их пришлось иным образом. Я также устанавливаю нужный бинарный файл.

5. Далее я создаю новый репозиторий на основе данного шаблона.

6. Создав новый репозиторий, я инициализирую chezmoi и порверяю, что всё работает правильно. Я также проверяю, что функция автоматического фиксирования и отправки изменений включена.

# Выводы

Выполнив эту лабораторную работу, я приобрёл опыт работы с несколькими полезными программами.

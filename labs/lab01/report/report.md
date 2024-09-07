---
## Front matter
title: "Отчёт по лабораторной работе № 1"
subtitle: "НКАбд-02-23"
author: "Выборнов Дмитрий Валерьевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
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

Целью работы является получение опыта работы с виртуальными машинами.

# Задание

- Установить и настроить виртуальную машину.

# Теоретическое введение

VirtualBox - это бесплатная и мощная программа, которая позволяет создавать и запускать виртуальные машины (VM) на вашем компьютере. Это означает, что вы можете запускать операционные системы, такие как Windows, Linux или macOS, прямо внутри вашей существующей операционной системы, как будто они установлены на отдельном компьютере.

# Выполнение лабораторной работы

1. Сначала я установил нужное ПО и скачал образ ОС для виртуальной машины.
2. После этого я настроил virtualbox и создал новую виртуальную машину при помощи этого образа.
3. В следующую очередь я настроил виртуальную машину, указав имя пользователя и установив програмное обеспечение для отчётов.

# Выводы

Выполнив эту лабораторную работу, я получил опыт работы с virtualbox.

# Контрольные вопросы

1. Учётная запись содержит такую информацию, как полное имя пользователя, пароль, электронную почту, группу, настройки, а также иногда дату рождения, телефонный номер и похожую персональную информацию.
2. Для получения справки по команде - man, для перемещения по файловой системе - cd, для просмотра содержимого каталога - ls, для определения объёма каталога - du, для создания / удаления каталогов / файлов - rm, для создания / удаления каталогов / файлов - chmod, для просмотра истории команд - history.
3. Файловая система - это способ организации и управления данными на компьютере. Она определяет структуру и иерархию файлов и каталогов, а также способы доступа к ним. Примеры: FAT (File Allocation Table): Простая и широко распространенная файловая система, использующаяся в Windows и других операционных системах, HFS+ (Hierarchical File System Plus): Файловая система, используемая в macOS. Она отличается своей простотой и надежностью, XFS (Extended File System): Файловая система, используемая в Linux.
4. Чтобы посмотреть, какие файловые системы подмонтированы в вашей операционной системе, можно использовать команду mount в консоли.
5. Удалить зависший процесс можно при помощи команды kill.

---
## Front matter
title: "Отчёт по лабораторной работе №4"
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

Целью этой лабораторной работы является приобретение практических навыков работы с git.

# Задание

Задание этой лабораторной работы заключается в правильном использовании git. 

# Теоретическое введение

 - Gitflow Workflow опубликована и популяризована Винсентом Дриссеном.
 - Gitflow Workflow предполагает выстраивание строгой модели ветвления с учётом выпуска проекта.
 - Данная модель отлично подходит для организации рабочего процесса на основе релизов.
 - Работа по модели Gitflow включает создание отдельной ветки для исправлений ошибок в рабочей среде.
 - Последовательность действий при работе по модели Gitflow:
 - Из ветки master создаётся ветка develop.
 - Из ветки develop создаётся ветка release.
 - Из ветки develop создаются ветки feature.
 - Когда работа над веткой feature завершена, она сливается с веткой develop.
 - Когда работа над веткой релиза release завершена, она сливается в ветки develop и master.
 - Если в master обнаружена проблема, из master создаётся ветка hotfix.
 - Когда работа над веткой исправления hotfix завершена, она сливается в ветки develop и master.

# Выполнение лабораторной работы

1. Сначала я установил всё необходимое ПО (git-flow, Node.js), после чего я настроил Node.js.
2. После этого я изменил формат коммитов, изменив файл package.json. 
3. После этого я приступил к конфигурации git-flow (при помощи git flow init) Я загрузил репозиторий в хранилище создал релиз и журнал изменений. После этого я залил релизную ветку в основную и отправил данные на github.
4. В последнюю очередь я создал новый релиз 1.2.3, обновил номер версии в файле package.json, создал список изменений и добавил его в индекс, залил релизную ветку в основную и отправил данные на github, после чего я создал релиз со списком изменений.

# Выводы

Выполнив эту лабораторную работу, я приобрёл навыки правильной работы с git. 

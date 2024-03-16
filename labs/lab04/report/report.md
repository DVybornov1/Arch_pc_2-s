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

Целью этой лабораторной работы является приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Задание

Задание этой лабораторной работы заключается в правильном использовании нескольких команд терминала Linux, таких, как, ls, cd, mkdir, rm и rmdir. 

# Теоретическое введение

В операционной системе типа Linux взаимодействие пользователя с системой обычно
осуществляется с помощью командной строки посредством построчного ввода команд. При этом обычно используется командные интерпретаторы языка shell: /bin/sh;
/bin/csh; /bin/ksh.
Командой в операционной системе называется записанный по
специальным правилам текст (возможно с аргументами), представляющий собой указание на выполнение какой-либо функций (или действий) в операционной системе.
Обычно первым словом идёт имя команды, остальной текст — аргументы или опции,
конкретизирующие действие.
Общий формат команд можно представить следующим образом:
<имя_команды><разделитель><аргументы>Использование символа «;». Если требуется выполнить последовательно несколько
команд, записанный в одной строке, то для этого используется символ точка с запятой.

# Выполнение лабораторной работы

1. Сначала я определил полное название своего домашнего каталога при помощи команды pwd.

2. В wsl в домашнем каталоге нет каталога /tmp, поэтому я демонстрировал работу команды ls на домашнем каталоге. Информация, которая выводится на экран этой программой изменяется в зависимости от используемых опций. Так, -a показывает скрытые файлы, а при помощи -l можно отобразит детальную информацию о содержимом содерхимого каталога, включая владельца и группу.

3. Я создаю новый каталог в домашнем каталоге, после чего внутри этого каталога создаю ещё один. После этого я использую команду mkdir, чтобы создать сразу три каталога, после чего я удатяю их примерно таким же образом, используя команду rmdir. Каталоги newdir и morefun при помощи rmdir одним действием удалить нельзя, так как в одном каталоге находится другой. Из - за этого я удаляю их, используя команду rm с опцией -r.

4. Я просматриваю доступные опции команды ls. За просмотр содержимого и основного каталога, и его подкаталогов, отвечает опция -R.

5. За сортировку выводимого командой ls списка по времени последнего изменення отвечает комбинация опций -tl.

6. У команды cd нет опций, у pwd две основные опции: -L активировать команду, даже если на пути есть символьные ссылки, и -P - избегать символьные ссылки. У команды mkdir основными опциями являются -m - установить владельца файла вручную, -p - создать "Родительские" каталоги, если их нет, и -v - выводить сообщение о каждом созданном каталоге. Команда rmd имеет 3 опции: -f - удалять всё, независимо от несуществующих файлов и других опций, -i - выводить сообщение перед каждым удалением, и -I - вывести одно сообщение, если удаляется более 3 файлов или удаление происходит рекурсивно. Команда rmdir имеет 2 опции: -p - удалить каталог вместе с его "Родительскими" каталогами и -v - выводить сообщение при каждом удалении каталога.

7. При помощи команды history я изменяю команды man и cd, которые я использовал до этого момента.

# Выводы

Выполнив эту лабораторную работу, я приобрёл навыки работы с системой при помощи командной строки. 

# Ответы на контрольные работы.

1. Командная строка - это программа, при помощи которой можно взаимодействовать с компьютером, вводя команды.

2. Определить абсолютный путь к текущему файлу можно найти при помощи команды pwd. Так, если использовать эту команду в домашнем каталоге, результатом будет /home/<username>/.

3. Определить только тип файлов и их имена в текущем каталоге можно при помощи комбинации опций -Fd.

4. Отобразить информацию о скрытых файлах можно при помощи команды ls с опцией -a.

5. Удалять файлы можно при помощи команд rm и rmdir, при чём при помощи команды rmdir можно удалять только каталоги.

6. Информацию о последних использованных командах можно при помощи команды history.

7. Для изменения ранее использованных команд неопходимо использовать команду history вот так: !номер команды:s/то, что нужно заменить/то, на что нужно заменить.

8. Несколько команд в одной строке можно запустить так: cd work; ls -a.

9. Символы экранирования используются для изменения принципа работы других символов и команд. Так, \n (Новая строка) - это символ экранирования.

10. При использовании опции -l выводится более детальная информация о содержимом каталога.

11. Относительный путь - путь из текущего каталога в нужный (src/helloworld), а абсолютный - путь в нужный каталог из домашнего (home/dvvybornov/src/helloworld).

12. Информацию о большинстве команд можно при помощи команды man.

13. Для автоматического дополнения вводимых команд служит клавиша tab. 
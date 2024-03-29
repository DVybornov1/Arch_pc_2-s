---
## Front matter
title: "Лабораторная работа №7"
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

# Цель работы.

Целью этой лабораторной работы является ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.


# Задание.

1. Команды для работы с файлами и каталогами.
2. Копирование файлов и каталогов.
3. Перемещение файлов и каталогов.
4. Права доступа.
5. Изменение прав доступа.
6. Анализ файловой системы.

# Теоретическое введение.

Для создания текстового файла можно использовать команду touch. Для просмотра файлов небольшого размера можно использовать команду cat. Для просмотра файлов постранично удобнее использовать команду less. Команда head выводит по умолчанию первые 10 строк файла.
Команда cp используется для копирования файлов и каталогов. Команды mv и mvdir предназначены для перемещения и переименования файлов
и каталогов. Права доступа к файлу или каталогу можно изменить, воспользовавшись командой
chmod. Файловая система в Linux состоит из фалов и каталогов. Каждому физическому носителю соответствует своя файловая система.
Существует несколько типов файловых систем. Для определения объёма свободного пространства на файловой системе можно воспользоваться командой df, которая выведет на экран список всех файловых систем
в соответствии с именами устройств, с указанием размера и точки монтирования.

# Выполнение лабораторной работы.

## Первый пункт.

Сначала я повторяю все примеры, указанные в первой части лабораторной работы. Из - за того, что я работаю в WSL, мне пришлось создать, переместить или изменить несколько файлов, чтобы правильно выполнить все задания.

## Второй пункт.

Я копирую файл asoundlib.h (единственный файл в каталоге sys/) в домашний каталог командой cp, после чего создаю новый каталог, перемещаю этот файл туда, и переименовываю его. После этого я создаю файл abc1 и копирую его в директорию ski.places, переименовывая его. Следующим действием я создаю новый каталог в каталоге ski.places, перемещаю туда файлы equiplist и equiplist2, создаю ещё один каталог и перемещаю его в каталог ski.places, переименовывая его plans.

## Третий пункт.

Для того, чтобы задать данным файлам такие разрешения нужно использовать команды chmod o+r,g+r,u+r,u+w,u+x australia, chmod o+x,g+x,u+x,u+w,u+r play, chmod o+r,g+r,u+r,u+x my_os, chmod o+r,g+r,g+w,u+r,u+w feathers.

## Четвёртый пункт.

Я просматриваю содержимое файла passwd (т. к. в WSL файл password называется так) при помощи команды cat. После этого я создаю новый файл, копирую в него файл feathers, перемещаю его в каталог play и перемещаю этот каталог в каталог games, попутно переименовывая его, при помощи mv. Далее я лишаю владельца файла feathers прав на чтение этого файла при помощи chmod и пытаюсь вывести его содержимое на экран при помощи команды cat и скопировать его, используя cp, но не могу этого сделать, так как я только что отобрал у себя же нужные для этого права. Я возвращаю владельцу файла feather права на его чтение, после чего лишаю владельца каталога play прав на выполнение, пытаюсь в него перейти и, ожидаемо, у меня ничего не получаегся, после чего я возвращаю себе нужные права.

## Пятый пункт.

1. Команда mount нужна для присоединения системы файлов с какого - то носителя к общей системе файлов компьютера. Эта команда используется так: mount (нужный девайс)**|(нужный каталог) -o (параметры, если они нужны)
2. Команда fsck нужна для проверки и починки файловых систем Linux. Она используется так: fsck (опции) (нужная система файлов)
3. Команда mkfs нужна для создания новых файловых систем. Она является частью многих "Создателей Систем Файлов" в Linux. Она используется так: mkfs (опции) -t (тип) (опции ф. с.) (девайс) (размер)
4. Команда kill посылает сигналы избранным процессам. Она работает так: kill (опции) (указатель нужных файлов)

# Выводы.

Выполнив эту лабораторную работу, я ознакомился с файловой системой Linux, её структурой, именами и содержанием
каталогов, приобрёл практические навыки по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами) и по проверке использования диска и обслуживанию файловой системы.

# Контрольные вопросы.

1. На жёстком диске моего компьютера находятся главные диски C: и D:, файловая система /dev/sdc, занимающая наибольшее количество блоков, системы rootfs и tmpfs, и много файловых систем, называющихся none и snapfuse.
2. Общая структура файловой системы Linux разделяется на несколько файловых систем, расположенных на разных дисках или устройствах и соединённых одним "Корнем". Каждая из этих систем разделяется на отдельные каталоги, где хранятся данные одного типа. Так, файлы программ хранятся в /usr/, а конфиг-файлы с настройками программ - в /etc/.
3. Для того, чтобы содержимое некотогой файловой структуры стало доступно операционной системе, необходимо изменить настройки монтирования этой системы файлов.
4. Основными причинами нарушения целостности файловых систем компьютера являются компьютерные вирусы, файлы и директории, удалённые, изменённые или перемещённые по ошибке, или неисправности/ошибки в коде программ, взаимодействующих с этими системами. Устранить повреждения файловых систем можно при помощи команды fsck.
5. Новые файловые системы создаются при помощи "Создателей Ф. С.", которые встроены в разные дистрибутивы Linux. Существует много создателей С. Ф., но большинство из них взаимосвязаны с командой mkfs.
6. Основной командой для просмотра текстовых файлов в Linux является cat. Также существует команда tac, делающая то же самое, что и cat, но в обратном порядке. Ещё существуют команды less, которая выводит текс более организованным образом (и используется как основа для команды man), head и tail, которые выводят некоторое количество строк с начала или конца файла, и grep, которая используется для поиска конкретных строк текста.
7. Команда cp в Linux используется в основном для копирования файлов. Она также может переименовывать файлы во время копирования.
8. Команда mv в Linux используется в основном для перемещения файлов. Она также может переименовывать файлы и каталоги и перезаписовать содержимое одного файла в другой.
9. Права доступа определяют то, кому дозволено делать с файлом те или иные вещи. Они разделяются на прова на чтение, изменение и исполнения и относятся отдельно к пользователю, группе пользователя и всем остальным. Права доступа можно изменить при помощи команды chmod.

# Библиография и ссылки.

1. GNU/Linux Pro (https://basis.gnulinux.pro/ru/latest/course.html#)

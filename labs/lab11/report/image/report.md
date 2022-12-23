---
## Front matter
title: "Отчёт по лабораторной работе №11"
subtitle: "*дисциплина: Архитектура компьютера*"
author: "Максим Александрович Мишонков"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью данной лабораторной работы является приобретение навыков написания программ для работы с файлами.

# Задание

Научиться писать программы для работы с файлами.

# Теоретическое введение

ОС GNU/Linux является многопользовательской операционной системой. И для обеспечения защиты данных одного пользователя от действий других пользователей существуют специальные механизмы разграничения доступа к файлам. Кроме ограничения доступа, данный механизм позволяет разрешить другим пользователям доступ данным для совместной работы.

Права доступа определяют набор действий (чтение, запись, выполнение), разрешённых для выполнения пользователям системы над файлами. Для каждого файла пользователь может входить в одну из трех групп: владелец, член группы владельца, все остальные. Для каждой из этих групп может быть установлен свой набор прав доступа. Владельцем файла является его создатель.

# Выполнение лабораторной работы

1. Создал каталог для программ лабораторной работы №11, перешёл в него и создал файлы lab11-1 и readme.txt. (рис. [-@fig:001])

![Создание каталога и файлов](image/Рис.1.png){ #fig:001 width=70% }

2. Ввёл в файл lab11-1.asm текст программы из листинга 11.1. Создал исполняемый файл и проверил его работу. Ответ сохранился в файле readme.txt. (рис. [-@fig:002], [-@fig:003], [-@fig:004])

![Введение текста программы](image/Рис.2.png){ #fig:002 width=70% }

![Введение текста программы](image/Рис.3.png){ #fig:003 width=70% }

![Проверка работы исполняемого файла](image/Рис.4.png){ #fig:004 width=70% }

3. С помощью команды chmod изменил права доступа к исполняемому файлу lab11-1, запретив его выполнение. В результате проверки работы исполняемого файла программа выдала отказ, как и следовало ожидать, так как запуск программы для владельца был запрещён. (рис. [-@fig:005])

![Запрет доступа к файлу](image/Рис.5.png){ #fig:005 width=70% }

4. С помощью команды chmod изменил права доступа к файлу lab11-1.asm с исходным текстом программы, добавив права на исполнение. В результате проверки работы исполняемого файла программа заработала, так как в файле были добавлены права на исполнение. (рис. [-@fig:006])

![Добавление прав на исполнение файла](image/Рис.6.png){ #fig:006 width=70% }

5. Предоставил права доступа к файлу readme.txt в соответствии с вариантом в таблице 11.4. Проверил правильность выполнения с помощью команды ls -l.(рис. [-@fig:007])

![Предотавление прав доступа к файлу](image/Рис.7.png){ #fig:007 width=70% }

**Самостоятельная работа** 

1. Написал программу, которая запрашивает имя и выводит его в созданном файле. Файл создаёт сама программа. (рис. [-@fig:008], [-@fig:009])

![Текст программы](image/Рис.8.png){ #fig:008 width=70% }

![Текст программы](image/Рис.9.png){ #fig:009 width=70% }

2. Создал исполняемый файл и проверил его работу. Проверил наличие файла и его содержимое с помощью команд ls и cat. (рис. [-@fig:010])

![Проверка работы исполняемого файла](image/Рис.10.png){ #fig:010 width=70% }

# Выводы

В ходе выполнения данной лабораторной работы я приобрёл навыки написания программ для работы с файлами.



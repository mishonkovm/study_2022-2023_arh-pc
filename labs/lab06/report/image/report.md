---
## Front matter
title: "Отчёт по лабораторной работе №6"
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

Целью данной лабораторной работы является приобретение практических навыков в Midnight Commander, освоение инструкций языка ассемблера mov и int.

# Задание

Приобретение практических навыков в Midnight Commander, освоение инструкций языка ассемблера mov и int.

# Теоретическое введение

**Midnight Commander (mc)** - это программа, которая позволяет просматривать структуру каталогов и выполнять основные операции по управлению файловой системой, т.е. mc является файловым менеджером.

Midnight Commander позволяет сделать работу с файлами более удобной и наглядной.

# Выполнение лабораторной работы

1. Открыл в терминале mc, перешёл в нужный каталог, с помощью функциональной клавиши F7 создал папку lab06 и перешёл в созданный каталог. (рис. [-@fig:001])

![Создание lab06](image/Рис.1.png){ #fig:001 width=70% }

2. Пользуясь строкой ввода и командой touch, создал файл lab6-1.asm. (рис. [-@fig:002], [-@fig:003])

![Создание файла lab6-1.asm](image/Рис.2.png){ #fig:002 width=70% }

![Создание файла lab6-1.asm](image/Рис.3.png){ #fig:003 width=70% }

3. С помощью функциональной клавиши F4 открыл файл lab6-1.asm для редактирования во встроенном редакторе mcedit, ввёл текст программы. (рис. [-@fig:004])

![Редактирование файла lab6-1.asm в mcedit](image/Рис.4.png){ #fig:004 width=70% }

4. Оттранслировал текст программы lab6-1.asm в объектный файл, выполнил компоновку объектного файла и запустите получившийся исполняемый файл. (рис. [-@fig:005])

![Оттранслирование текста в объектный файл, его компановка и запуск](image/Рис.5.png){ #fig:005 width=70% }

5. Переместил файл in_out.asm в каталог с файлом lab6-1.asm с помощью функциональной клавиши F6. (рис. [-@fig:006], [-@fig:007]) 

![Перемещение файла in_out.asm в каталог с файлом lab6-1.asm](image/Рис.6.png){ #fig:006 width=70% }

![Перемещение файла in_out.asm в каталог с файлом lab6-1.asm](image/Рис.7.png){ #fig:007 width=70% }

6. С помощью функциональной клавиши F5 создал копию файла lab6-1.asm с именем lab6-2.asm. (рис. [-@fig:008], [-@fig:009])

![Создание копии файла lab6-1.asm](image/Рис.8.png){ #fig:008 width=70% }

![Создание копии файла lab6-1.asm](image/Рис.9.png){ #fig:009 width=70% }

7. Исправил текст программы в файле lab6-2.asm, создал исполняемый файл и проверил его работу. (рис. [-@fig:010], [-@fig:011])

![Исполнение текста программы](image/Рис.10.png){ #fig:010 width=70% }

![Проверка работы файла](image/Рис.11.png){ #fig:011 width=70% }

8. В файле lab6-2.asm заменил подпрограмму sprintLF на sprint, создал исполняемый файл и проверил его работу. (рис. [-@fig:012], [-@fig:013])

![Замена подпрограммы](image/Рис.12.png){ #fig:012 width=70% }

![Проверка работы файла](image/Рис.13.png){ #fig:013 width=70% }

**Самостоятельная работа**

1. Создал копию файла lab6-1.asm, внёс изменения в программу. (рис. [-@fig:014], [-@fig:015], [-@fig:016])

![Создание копии файла](image/Рис.14.png){ #fig:014 width=70% }

![Создание копии файла](image/Рис.15.png){ #fig:015 width=70% }

![Изменения](image/Рис.16.png){ #fig:016 width=70% }

2. Проверил работу файла. (рис. [-@fig:017])

![Проверка работы файла](image/Рис.17.png){ #fig:017 width=70% }

3. Создал копию файла lab6-2.asm, внёс изменения в программу. (рис. [-@fig:018], [-@fig:019], [-@fig:020])

![Создание копии файла](image/Рис.18.png){ #fig:018 width=70% }

![Создание копии файла](image/Рис.19.png){ #fig:019 width=70% }

![Изменения](image/Рис.20.png){ #fig:020 width=70% }

4. Проверил работу файла. (рис. [-@fig:021])

![Проверка работы файла](image/Рис.21.png){ #fig:021 width=70% }

# Выводы

В ходе выполнения данной лабораторной работы я приобрёл практические навыки работы с Midnight Commander, освоил инструкции языка ассемблера mov и int.




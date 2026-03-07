---
## Front matter
title: "Лабораторная работа №1"
subtitle: "дисциплина: Архитектура компьютера"
author: "Татур Платон Андреевич"

## Generic otions
lang: ru-RU\
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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

- Установка Linux Fedora Sway на виртуальную машину
- Установка необходимого для работы программного обеспечения
- Первоначальная настройка операционной системы

# Теоретическое введение

# Выполнение лабораторной работы

создаю новую виртуальную машину в virt manager (рис. -@fig:001)

![Создание виртуальной машины](./image/1.png){#fig:001 width=70%}

Через liveins задаю базовые настройки для установки операционной системы. (рис. -@fig:002)

![Процесс установки](./image/2.png){#fig:002 width=70%}

Скачиваю набор пакетов для работы с ОС.(рис. -@fig:003)

![Установка ПО](./image/3.png){#fig:003 width=70%}

Запускаю скрипт для автоматического обновления пакетов через пакетный менеджер dnf.. (рис. -@fig:004)

![Запуск скрипта](./image/4.png){#fig:004 width=70%}

Отключаю защиту SELinux. (рис. -@fig:005)

![Отключение защиты Linux](./image/5.png){#fig:005 width=70%}

Настраиваю xkb, добавляю вторую раскладку клавиатуры с русским языком и задаю переключение на right ctrl. (рис. -@fig:006)

![Настройка xkb](./image/6.png){#fig:006 width=70%}

Проверяю корректность заданного имени для hostname. (рис. -@fig:007)

![Вывод команды hostnamectl](./image/7.png){#fig:007 width=70%}

Устанавливаю pandoc, pandoc-crossref и texlive. (рис. -@fig:008)

![Установка pandoc pandoc-crossref и texlive](./image/8.png){#fig:008 width=70%}

# Домашнее задание

Выводы команды dmesg с разными аргументами (рис. -@fig:009)

![Вывод команды dmesg](./image/9.png){#fig:009 width=70%}

Выводы команды dmesg с разными аргументами (рис. -@fig:010)

![Вывод команды dmesg](./image/10.png){#fig:010 width=70%}

Выводы команды dmesg с разными аргументами (рис. -@fig:011)

![Вывод команды dmesg](./image/11.png){#fig:011 width=70%}


# Выводы

В ходе выполнения лабораторный работы приборел навыки установки виртуальной машины, установил ряд пакетов и настроил ОС для дальнейшей работы на ней.

# Список литературы{.unnumbered}

::: {#refs}
:::

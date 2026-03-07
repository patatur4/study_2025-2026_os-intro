---
## Front matter
title: "Лабораторная работа №4"
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

Получение навыков продвинутой работы с репозиториями git и релизами.

# Задание

- Работу с тестовым репозиторием.
- Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits.

# Теоретическое введение

Gitflow Workflow — это одна из самых известных и долгое время популярных моделей ветвления (branching model) в Git. Она была предложена Винсентом Дриссеном в 2010 году в статье «A successful Git branching model» и на многие годы стала фактически стандартом для команд, работающих с версионными релизами.

# Выполнение лабораторной работы

Устанавливаю nodejs. (рис. -@fig:001)

![Установка nodejs](image/1.png){#fig:001 width=70%}

Устанавливаю pnpm. (рис. -@fig:002)

![Установка pnpm](image/2.png){#fig:002 width=70%}

Устанавливаю gitflow. (рис. -@fig:003)

![Установка gitflow](image/3.png){#fig:003 width=70%}

С помощью pnpm устанавливаю commitizen и standard-changelog. (рис. -@fig:004)

![Установка с помощью pnpm](image/4.png){#fig:004 width=70%}

Создаю новый репозиторий и делаю там первый commit. (рис. -@fig:005)

![Создание репозитория и первый commit](image/5.png){#fig:005 width=70%}

Редактирую package.json. (рис. -@fig:006)

![Отредактированный файл package.json](image/6.png){#fig:006 width=70%}

Отправляю commit на GitHub (рис. -@fig:007)

![Отправление commit на GitHub](image/7.png){#fig:007 width=70%}

Инициализирую в репозитории git flow и создаю один релиз созданной ветке develop. (рис. -@fig:008)

![Использование git-flow](image/8.png){#fig:008 width=70%}

Создаю список изменений через standard changelog, заканчиваю релиз и выгружаю на удаленный репозиторий изменения. (рис. -@fig:009)

![Загрузка релиза на github](image/9.png){#fig:009 width=70%}

Инициализирую ветку feature для работы над новой функциональностью, готовлю релиз и загружаю на github. (рис. -@fig:010)

![Работа с новой веткой и загрузка релиза](image/10.png){#fig:010 width=70%}

# Выводы

В ходе выполнения лабораторный работы я получил навыки правильной работы с репозиториями git.

# Список литературы{.unnumbered}

::: {#refs}
:::

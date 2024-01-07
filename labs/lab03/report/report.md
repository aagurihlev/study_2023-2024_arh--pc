---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Язык разметки Markdown"
author: "Гурылев Артем Андреевич"

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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы

Откроем терминал(рис. @1):

![Терминал](image/1.png){#fig:1}

Зайдем в рабочий каталог, после чего обновим его содержание командой git pull(рис. @2):

![Обновление каталога с помощью git](image/2.png){#fig:2}

Перейдём в каталог с шаблоном отчета по лабораторной работе № 3(рис. @3): 

![Каталог лабораторной работы №3](image/3.png){#fig:3}

Проведём компиляцию шаблона с помощью Makefile, и убедимся в генерации файлов docx и pdf(рис. @4):

![Компиляция шаблона](image/4.png){#fig:4}

Удалим полученные файлы используя Makefile, и убедимся в их отсутствии(рис. @5):

![Удаление файлов с помощью make](image/5.png){#fig:5}

Откроем файл и заполним отчет по шаблону, после чего загрузим файлы на Github(рис. @6, @7):

![Загрузка файлов в репозиторий](image/6.png){#fig:6}

![Загрузка файлов в репозиторий](image/7.png){#fig:7}

# Выполнение самостоятельной работы

Заполним отчет для второй лабораторной работы и скомпилируем его(рис. @8)

![Компиляция файла](image/8.png){#fig:8}

Загрузим файлы на Github(рис. @9):

![Загрузка файлов в репозиторий](image/9.png){#fig:9}

# Выводы

В данной лабораторной работе я научился работать с языком разметки Markdown, а также компилировать отчет для лабораторных работ, используя Pandoc и Latex.


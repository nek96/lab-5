---
# Front matter
title: "Отчёт по лабораторной работе №5"
subtitle: “Алгоритмы в программировании”
author: "Некпаи Амруддин"
institute: RUDN University, Moscow, Russian Federation
# Generic otions
lang: ru-RU
toc-title: "Содержание"

# Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
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
## Misc options
indent: true
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью этой работы является изучение и понимание алгоритмов в контексте программирования. Алгоритмы играют важную роль в создании эффективных и оптимизированных программ. Они представляют собой последовательность инструкций, которые решают определенную задачу.

# Выполнение работы

В ходе работы были изучены различные типы алгоритмов, включая алгоритмы сортировки, поиска, графические алгоритмы, алгоритмы машинного обучения и алгоритмы оптимизации. Были рассмотрены примеры каждого типа алгоритма и обсуждены их применения.

Также была проведена работа над пониманием временной сложности алгоритма, которая определяет, как быстро алгоритм может решить задачу. Это особенно важно для больших наборов данных, где эффективный алгоритм может значительно ускорить процесс.

Алгоритм сортировки пузырьком:
Python
AI-generated code. Review and use carefully. More info on FAQ.

def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
    return arr
Линейный поиск:
Python
AI-generated code. Review and use carefully. More info on FAQ.

def linear_search(arr, x):
    for i in range(len(arr)):
        if arr[i] == x:
            return i
    return -1
Бинарный поиск:
Python
AI-generated code. Review and use carefully. More info on FAQ.

def binary_search(arr, low, high, x):
    if high >= low:
        mid = (high + low) // 2
        if arr[mid] == x:
            return mid
        elif arr[mid] > x:
            return binary_search(arr, low, mid - 1, x)
        else:
            return binary_search(arr, mid + 1, high, x)
    else:
        return -1

# Выводы
Алгоритмы являются неотъемлемой частью программирования. Они помогают программистам решать сложные задачи более эффективно и оптимизированно. Понимание различных типов алгоритмов и их применений может значительно улучшить навыки программирования.

# Список литературы{.unnumbered}

Кормен, Томас Х. и др. “Алгоритмы: построение и анализ”. 3-е изд. М.: Вильямс, 2016.
Седжвик, Роберт. “Алгоритмы на Java”. 4-е изд. М.: ДМК Пресс, 2011.
Грокаем алгоритмы. Адитья Бхаргава. М.: Питер, 2017.


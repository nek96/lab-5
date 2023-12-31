---
## Front matter
lang: ru-RU
title: "Отчёт по лабораторной работе №5"
title: "Алгоритмы в программировании"
author: Некпаи Амруддин
institute: Российский Университет Дружбы Народов
date: 22 октября, 2023, Москва, Россия

## Formatting
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true

---

# Цели и задачи

## Цель лабораторной работы
Целью этой работы является изучение и понимание алгоритмов в контексте программирования. Алгоритмы играют важную роль в создании эффективных и оптимизированных программ. Они представляют собой последовательность инструкций, которые решают определенную задачу.

# Выполнение лабораторной работы

 В ходе работы были изучены различные типы алгоритмов, включая алгоритмы сортировки, поиска, графические алгоритмы, алгоритмы машинного обучения и алгоритмы оптимизации. Были рассмотрены примеры каждого типа алгоритма и обсуждены их применения.

Также была проведена работа над пониманием временной сложности алгоритма, которая определяет, как быстро алгоритм может решить задачу. Это особенно важно для больших наборов данных, где эффективный алгоритм может значительно ускорить процесс.



## Пример работы алгоритма

Конечно, вот несколько базовых алгоритмов, реализованных на Python:

1. **Алгоритм сортировки пузырьком**:
```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
    return arr
```

2. **Линейный поиск**:
```python
def linear_search(arr, x):
    for i in range(len(arr)):
        if arr[i] == x:
            return i
    return -1
```

3. **Бинарный поиск**:
```python
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
```


# Выводы
Алгоритмы являются неотъемлемой частью программирования. Они помогают программистам решать сложные задачи более эффективно и оптимизированно. Понимание различных типов алгоритмов и их применений может значительно улучшить навыки программирования.


## список летиратур
Кормен, Томас Х. и др. “Алгоритмы: построение и анализ”. 3-е изд. М.: Вильямс, 2016.
Седжвик, Роберт. “Алгоритмы на Java”. 4-е изд. М.: ДМК Пресс, 2011.
Грокаем алгоритмы. Адитья Бхаргава. М.: Питер, 2017.


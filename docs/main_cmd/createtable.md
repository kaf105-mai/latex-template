---
layout: default
title: Вставка таблицы
parent: Основные команды
nav_order: 5
---

# Команда createtable
Команда принимает на вход 3 аргумента.

```latex
\createtable{Название}{label}{каркас таблицы}
```

где 

* ```Название``` - название таблицы
* ```label``` - название таблицы для возможности цитирования
* ```Каркас таблицы``` - каркас таблицы

Пример

```latex
\createtable
{Анализ роста числа параметров при развитии моделей глубокого обучения}
{tb:dl_model}
{
    \begin{tabular}{|l|l|l|l|l}
    \hline
    Название               & AlexNet     & VGGNet      & ResNet      & BERT       \\ \hline
    Год                          & 2012        & 2014        & 2015        & 2018      \\ \hline
    Тип данных             & изображение & изображение & изображение & текст     \\ \hline
    Число параметров, млрд & $0{,}06$    & $0{,}13$    & $0{,}06$    & $0{,}34$  \\ \hline
    \end{tabular}
}
```



Исходный код

```latex
\newcommand{\createtable}[3]{
    \begin{table}[!ht]
        \caption{#1}
        \label{#2}
        \begin{center}
            \resizebox{\textwidth}{!}{
                {#3}
            }
        \end{center}
    \end{table}
}
```
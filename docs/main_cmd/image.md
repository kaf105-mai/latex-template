---
layout: default
title: Вставка изображений
parent: Основные команды
nav_order: 2
---

# Команда image

Команда принимает на вход 4 аргумента.

```latex
\image{PATH_TO_IMG}{Название}{label}{scale}
```

где 

* ```PATH_TO_IMG``` - путь до изображения. Например, ```src/img/*.jpg```
* ```Название``` - название изображения 
* ```label``` - название изображения для возможности цитирования
* ```scale``` - изменяет размер изображения

Пример 

```latex
\image{docs/img/logo.jpg}
{Символика МАИ}
{img:logo}
{0.35}
```

Исходный код

```latex
\newcommand{\image}[4]{
    \begin{figure}[!ht]\center
    \includegraphics[width=#4\textwidth]{#1}
    \caption{#2}
    \label{#3}
    \end{figure}
}
```
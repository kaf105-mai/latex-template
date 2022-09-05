---
layout: default
title: Вставка теоремы
parent: Основные команды
nav_order: 4
---

# Команда createtheorem
Команда принимает на вход 2 аргумента.

```latex
\createtheorem{label}{text}
```

где 

* ```label``` - название теоремы для возможности цитирования
* ```text``` - текст теоремы

Пример

```latex
\createtheorem
{th:helm}
{
    В непрерывных течениях идеального газа напряжения вихревого жгута с течением времени не изменяется
}
```



Исходный код

```latex
\newcommand{\createtheorem}[2]{
    \begin{theorem}
    \label{#1}
        {#2}
    \end{theorem}
}
```

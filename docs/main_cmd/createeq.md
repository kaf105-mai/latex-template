---
layout: default
title: Вставка уравнения
parent: Основные команды
nav_order: 3
---

# Команда createeq
Команда принимает на вход 2 аргумента.

```latex
\createeq{label}{text}
```

где 

* ```label``` - название уравнения для возможности цитирования
* ```text``` - текст уравнения

Пример

```latex
\createeq
{eq:cya}
{
    C_{y_a} = \frac{Y_a}{qS}
}
```



Исходный код

```latex
\newcommand{\createeq}[2]{
   \begin{gather}
    \label{#1}
        \begin{aligned}
            {#2}
        \end{aligned}
    \end{gather}
}
```
---
layout: default
title: Вставка главы без нумерации
parent: Основные команды
nav_order: 1
---

# Команда chapterbul

Команда принимает на вход 2 аргумента.

```latex
\chapterbul{Название}{PATH_TO_TEX}
```

где 

* ```Название``` - название главы 
* ```PATH_TO_TEX``` - путь до файла с расширением tex

Пример
```latex
\chapterbul{Введение}{src/1-text/0-intro}
```

Исходный код

```latex
\newcommand{\chapterbul}[2]{
    \newpage
    \addcontentsline{toc}{section}{#1}
    \chapter*{#1}
    \input{#2}
}
```
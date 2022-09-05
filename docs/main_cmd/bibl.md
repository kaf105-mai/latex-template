---
layout: default
title: Вставка списка источников
parent: Основные команды
nav_order: 8
---

# Команда bibl
Команда принимает на вход 1 аргумент.

Оформление списка источников согласно ГОСТ 7.1 (ГОСТ Р 7.0.11-2011, 5.6.7).

Оформление в формате BibTeX.

```latex
\bibl{PATH_TO_BIB}
```

где 

* ```PATH_TO_BIB``` - путь до файла с расширением bib

Пример

```latex
\bibl{src/2-bib/refs.bib}
```

Исходный код

```latex
\newcommand{\bibl}[1]{
    \newpage
    \addcontentsline{toc}{section}{Список литературы}
    \renewcommand{\bibname}{Список литературы}
    \nocite{*}
    \bibliography{#1}
}
```


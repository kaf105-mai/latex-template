---
layout: default
title: Главная
permalink: /
---

За основу шаблона была взята диссертация Грабового А.В. [github](https://github.com/andriygav/PhDThesis)

Шаблон был реструктизирован:

* Добавлены папки settings и src:
    
    - settings содержит преамбулу, макросы, и файл bst для оформления библиографических ссылок по ГОСТ
    - src содержит папки с tex-файлами

        * 0-title: титульные листы
        * 1-text: главы
        * 2-bib: файл с расширением bib и шаблон для ручного внесения источника
        * appendix: вывод и нотация
        * img: изображения

* Добавлены [макросы](https://kaf105-mai.github.io/latex-template/latex-template/main_cmd/) для удобства работы с таблицами, уравнениями, теоремами

Шаблон разработан для использование в онлайн редакторе [overleaf](https://www.overleaf.com/latex/templates/template-kaf105-mai-for-report/ypzjzmbntpyw)

Разработал магистр 105 кафедры [Ли Яков](https://t.me/leeyakov)

Документация написана на Jekyll с темой [just the docs](https://just-the-docs.github.io/just-the-docs/)
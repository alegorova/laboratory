---
# Front matter
lang: ru-RU
title: "Лабораторная работа №3"
subtitle: "Дисциплина: Операционные системы"
author: "Егорова Александра"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
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

Изучить идеологию и применение средств контроля версий.

# Задание

Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.

# Выполнение лабораторной работы

Создаем учётную запись на https://github.com. (рис. -@fig:001)

![Рис.1](images/1.png){ #fig:001 width=70% }

Настраиваем систему контроля версий git. Синхранизируем учётную
запись github с компьютером:
git config --global user.name "Имя Фамилия"
git config --global user.email "work@mail" (рис. -@fig:002)

![Рис.2](images/2.png){ #fig:002 width=70% }

Создаем новый ключ на github и привязываю его к компьютеру через консоль. (рис. -@fig:003) (рис. -@fig:004) (рис. -@fig:005) (рис. -@fig:006) 

![Рис.3](images/3.png){ #fig:003 width=70% }
![Рис.4](images/4.png){ #fig:004 width=70% }
![Рис.5](images/5.png){ #fig:005 width=70% }
![Рис.6](images/6.png){ #fig:006 width=70% }

Подключение репозитория к github.Заходим в «repositories» и создаем новый репозиторий (имя «labor2»). (рис. -@fig:007)
Копируем в консоль ссылку на репозиторий.(рис. -@fig:008)

![Рис.7](images/7.png){ #fig:007 width=70% }
![Рис.8](images/8.png){ #fig:008 width=70% }

Работаем с каталогом и папками через консоль.(рис. -@fig:009) Создаем файлы. (рис. -@fig:010)

![Рис.9](images/9.png){ #fig:009 width=70% }
![Рис.10](images/10.png){ #fig:010 width=70% }

Добавляем первый коммит и выкладываем на githup. Чтобы правильно разместить первый коммит, необходимо добавить команду git add . , далее с помощью команды git commit -am "first commit" выкладываем коммит. (рис. -@fig:011)
Сохраняем первый коммит (git push). (рис. -@fig:012)

![Рис.11](images/11.png){ #fig:011 width=70% }
![Рис.12](images/12.png){ #fig:012 width=70% }

Первичная конфигурация. Добавим файл лицензии. (рис. -@fig:013)

![Рис.13](images/13.png){ #fig:013 width=70% }

Добавим шаблон игнорируемых файлов. Получим список имеющихся шаблонов (на скрине представлены не все шаблоны). (рис. -@fig:014)

![Рис.14](images/14.png){ #fig:014 width=70% }

Затем скачаем шаблон, например, для C. Также добавим новые файлы и выполним коммит. (рис. -@fig:015)
Отправляем на github (git push). (рис. -@fig:016)

![Рис.15](images/15.png){ #fig:015 width=70% }
![Рис.16](images/16.png){ #fig:016 width=70% }

Конфигурация git-flow. Инициализируем git-flow с помощью команды git flow init -f. Префикс для ярлыков установим в v. (рис. -@fig:017)

![Рис.17](images/17.png){ #fig:017 width=70% }

Проверяем, что находимся на ветке develop (git branch). (рис. -@fig:018)

![Рис.18](images/18.png){ #fig:018 width=70% }

Создадим релиз с версией 1.0.0. (рис. -@fig:019)
Запишем версию и добавим в индекс. (рис. -@fig:020)

![Рис.19](images/19.png){ #fig:019 width=70% }
![Рис.20](images/20.png){ #fig:020 width=70% }

Зальём релизную ветку в основную ветку. (рис. -@fig:021)
Отправим данные на github. (рис. -@fig:022)

![Рис.21](images/21.png){ #fig:021 width=70% }
![Рис.22](images/22.png){ #fig:022 width=70% }

Создаем релиз на github. Заходим в «Releases», нажимаем «Создать новый релиз». Заходим в теги и заполняем все поля. (рис. -@fig:023) После создания тега, автоматически сформируется релиз. (рис. -@fig:024)

![Рис.23](images/23.png){ #fig:023 width=70% }
![Рис.24](images/24.png){ #fig:024 width=70% }

# Выводы

В ходе выполнения лабораторной работы я изучила идеологию и применение средств контроля версий.

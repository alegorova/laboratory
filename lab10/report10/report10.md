---
# Front matter
lang: ru-RU
title: "Лабораторная работа №10"
subtitle: "Дисциплина: Операционные системы"
author: "Егорова Александра"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Задание

1. Ознакомиться с теоретическим материалом.
2. Ознакомиться с редактором emacs.
3. Выполнить упражнения.
4. Ответить на контрольные вопросы

# Выполнение лабораторной работы

Для работы с Emacs необходимо установить данный редактор,используя команду "sudo yum install emacs". (рис. -@fig:001)

![Установка emacs](images10/1.png){ #fig:001 width=70% }

1) Откроем редактор Emacs с помощью команды «emacs &». (рис. -@fig:002) (рис. -@fig:003)

![Редактор Emacs](images10/2.png){ #fig:002 width=70% }

![Редактор Emacs](images10/3.png){ #fig:003 width=70% }

2) Создадим файл lab10.sh с помощью комбинации «Ctrl-x» «Ctrl-f». (рис. -@fig:004)

![Создаем файл](images10/4.png){ #fig:004 width=70% }

3) В открывшемся буфере наберем необходимый текст. (рис. -@fig:005)

![Вводим текст](images10/5.png){ #fig:005 width=70% }

4) Сохраним файл с помощью комбинации «Ctrl-x» «Ctrl-s».
5)Проделаем с текстом стандартные процедуры редактирования, каждое действие должно осуществляться комбинацией клавиш.
5.1) Вырежем одной командой целую строку («Сtrl-k»). (рис. -@fig:006)

![Вырезаем строку](images10/6.png){ #fig:006 width=70% }

5.2) Вставим эту строку в конец файла («Ctrl-y»). (рис. -@fig:007)

![Вставляем строку](images10/7.png){ #fig:007 width=70% }

5.3) Выделим область текста («Ctrl-space»). (рис. -@fig:008)

![Выделим область](images10/8.png){ #fig:008 width=70% }

5.4) Скопируем область в буфер обмена («Alt-w»).
5.5) Вставим область в конец файла («Ctrl-y»). (рис. -@fig:009)

![Вставим область](images10/9.png){ #fig:009 width=70% }

5.6) Вновь выделим эту область («Ctrl-space») (Рисунок 9) и на этот раз вырежем её («Ctrl-w»). (рис. -@fig:010)

![Скопируем и вставим область](images10/10.png){ #fig:010 width=70% }

5.7) Отменим последнее действие («Ctrl-x u»). (рис. -@fig:011)

![Отмена последнего действия](images10/11.png){ #fig:011 width=70% }

6) Научимся использовать команды по перемещению курсора.
6.1) Переместим курсор в начало строки («Ctrl-a»). (рис. -@fig:012)

![Перемещение курсора](images10/12.png){ #fig:012 width=70% }

6.2) Переместим курсор в конец строки («Ctrl-e»). (рис. -@fig:013)

![Перемещение курсора](images10/13.png){ #fig:013 width=70% }

6.3) Переместим курсор в начало буфера («Alt-<»). (рис. -@fig:014)

![Перемещение курсора](images10/14.png){ #fig:014 width=70% }

6.4) Переместим курсор в конец буфера («Alt->»). (рис. -@fig:015)

![Перемещение курсора](images10/15.png){ #fig:015 width=70% }

7) Управление буферами.
7.1) Выведем список активных буферов на экран («Ctrl-x» «Ctrl-b»). (рис. -@fig:016)

![Список активных буферов](images10/16.png){ #fig:016 width=70% }

7.2) Переместимся во вновь открытое окно («Ctrl-x o») со списком открытых буферов и переключимся на другой буфер (для этого необходимо нажать на «enter» после выбора необходимого буфера). (рис. -@fig:017)

![Список активных буферов](images10/17.png){ #fig:017 width=70% }

7.3) Закроем это окно («Ctrl-x 0»). (рис. -@fig:018)

![Закрываем окно](images10/18.png){ #fig:018 width=70% }

7.4) Теперь вновь переключимся между буферами, но уже без вывода их списка на экран («Ctrl-x b»). (рис. -@fig:019) (рис. -@fig:020)

![Переключимся между буферами](images10/19.png){ #fig:019 width=70% }

![Переключимся между буферами](images10/20.png){ #fig:020 width=70% }

8) Управление окнами
8.1) Поделим фрейм на 4 части: разделим фрейм на два окна по вертикали («Ctrl-x 3»), а затем каждое из этих окон на две части по горизонтали («Ctrl-x 2»). (рис. -@fig:021) (рис. -@fig:022) (рис. -@fig:023)

![Разделение фрейма](images10/21.png){ #fig:021 width=70% }

![Разделение фрейма](images10/22.png){ #fig:022 width=70% }

![Разделение фрейма](images10/23.png){ #fig:023 width=70% }

8.2) В каждом из четырёх созданных окон откроем новый буфер (файл) и введем несколько строк текста. Для этого предварительно создадим эти файлы с помощью команд «touch example1.txt», «touch example2.txt», «touch example3.txt», «touch example4.txt». (рис. -@fig:024) (рис. -@fig:025)

![Создаем файлы](images10/24.png){ #fig:024 width=70% }

![Вводим текст](images10/25.png){ #fig:025 width=70% }

9) Режим поиска
9.1) Переключимся в режим поиска («Ctrl-s») и найдем несколько слов, присутствующих в тексте. (рис. -@fig:026) (рис. -@fig:027)

![Переключимся в режим поиска](images10/26.png){ #fig:026 width=70% }

![Найдем несколько слов](images10/27.png){ #fig:027 width=70% }

9.2) Переключимся между результатами поиска, нажимая «Ctrl-s». (рис. -@fig:028)

![Переключимся между результатами поиска](images10/28.png){ #fig:028 width=70% }

9.3) Выйдем из режима поиска, нажав «Ctrl-g». (рис. -@fig:029)

![Выйдем из режима поиска](images10/29.png){ #fig:029 width=70% }

9.4) Перейдем в режим поиска и замены («Alt-%»), введем текст, который следует найти и заменить, нажмем «enter», затем введем текст для замены. После того как будут подсвечены результаты поиска, нажмем «!» для подтверждения замены. Важно, чтобы курсор находился в начале текста. (рис. -@fig:030) (рис. -@fig:031) (рис. -@fig:032) (рис. -@fig:033)

![Замена текста](images10/30.png){ #fig:030 width=70% }

![Замена текста](images10/31.png){ #fig:031 width=70% }

![Замена текста](images10/32.png){ #fig:032 width=70% }

![Замена текста](images10/33.png){ #fig:033 width=70% }

9.5) Пробуем другой режим поиска, нажав «Alt-s o». (рис. -@fig:034) (рис. -@fig:035)

![Другой режим поиска](images10/34.png){ #fig:034 width=70% }

![Другой режим поиска](images10/35.png){ #fig:035 width=70% }

# Выводы

В ходе выполнения данной лабораторной работы я познакомилась с операционной системой Linux и получила практические навыки работы с редактором Emacs.

# Контрольные вопросы

1) Emacs − один из наиболее мощных и широко распространённых редакторов, используемых в мире Unix. По популярности он соперничает с редактором vi и его клонами. В зависимости от ситуации, Emacs может быть:а) текстовым редактором;б) программой для чтения почты и новостей Usenet; в) интегрированной средой разработки (IDE); г) операционной системой и т.д. Всё это разнообразие достигается благодаря архитектуре Emacs, которая позволяет расширять возможности редактора при помощи языка Emacs Lisp. На языке C написаны лишь самые базовые и низкоуровневые части Emacs, включая полнофункциональныйинтерпретатор языка Lisp. Таким образом, Emacs имеет встроенный язык программирования, который может использоваться для настройки, расширения и изменения поведения редактора. В действительности, большая часть того редактора, с которым пользователи Emacs работают в наши дни, написана на языке Lisp.

2) Основную трудность для новичков при освоении данного редактора могут составлять большое количество команд, комбинаций клавиш, которые не получится все запомнить с первого раза и поэтоу придется часто обращаться к справочным материалам.

3) Буфер – это объект, представляющий собой текст. Если имеется несколько буферов, то редактировать можно только один. Обычно буфер считывает данные из файла или записывает в файл данные из буфера. Окно – это область экрана, отображающая буфер. При запуске редактора отображается одно окно, но при обращении к некоторым функциям могут открыться дополнительные окна. Окна Emacs и окна графической среды X Window – разные вещи. Одно окно X Window может быть разбито на несколько окон в смысле Emacs, в каждом из которых отображается отдельный буфер.

4) Да, можно.

5) При запуске Emacs по умолчанию создаются следующие буферы: а) «scratch» (буфер для несохраненного текста); б) «Messages» (журнал ошибок, включающий также информацию, которая появляется в области EchoArea); в) «GNU Emacs» (справочный буфер о редакторе).

6) C-c | сначала, удерживая «ctrl», нажимаю «c», после – отпускаю обе клавиши и нажимаю «|». C-c C-| сначала, удерживая «ctrl», нажимаю «с», после – отпускаю обе клавиши и, удерживая «ctrl», нажимаю «|»

7) Чтобы поделить окно на две части необходимо воспользоваться комбинацией «Ctrl-x 3» (по вертикали) или «Ctrl-x 2» (по горизонтали).

8) Настройки Emacs хранятся в файле .emacs.

9) По умолчанию клавиша «←» удаляет символ перед курсором, но в редакторе её можно переназначить. Для этого необхдимо изменить конфигурацию файла .emacs.

10) Более удобным я считаю редактор emacs, потому что в нем проще открывать другие файлы, можно использовать сразу несколько окон, нет «Командного режима», «Режима ввода», «Режима командной строки», которые являются немного непривычными и в какой-то степени неудобными.


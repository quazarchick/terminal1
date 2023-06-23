Первая часть первого  ДЗ  ))
Linux terminal (GitBash) commands

1) Посмотреть где я  - pwd
2) Создать папку - mkdir papka
3) Зайти в папку - cd papka
4) Создать 3 папки - $ mkdir papka_1 papka_2 papka_3
5) Зайти в любоую папку - cd papka_1
6) Создать 5 файлов (3 txt, 2 json) - touch 1.txt 2.txt 3.txt 4.json 5.json
7) Создать 3 папки - mkdir papka_4 papka_5 papka_6
8) Вывести список содержимого папки - ls -la
9) + Открыть любой txt файл - $ nano 1.txt
10) + написать туда что-нибудь, любой текст. - abracadabra
11) + сохранить и выйти. Ctrl + X, Y
12) Выйти из папки на уровень выше - $ cd ..
—
13) переместить любые 2 файла, которые вы создали, в любую другую папку. $ mv 1.txt 2.txt ~/Desktop/papka_2
14) скопировать любые 2 файла, которые вы создали, в любую другую папку. $ cp 1.txt 2.txt ~/Desktop/papka_3
15) Найти файл по имени $ find -name 1.txt
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. - $ tail -v 1.txt
17) вывести несколько первых строк из текстового файла - $ head -n 1 1.txt
18) вывести несколько последних строк из текстового файла - $ tail -n 3 1.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает - $ less 1.txt
20) вывести дату и время - $ date
=========

Задание *
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request

$ curl http://162.55.220.72:5006/terminal-hw-request


2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

#!/bin/bash
cd papka mkdir papka_1 papka_2 papka_3
cd papka_1
touch 1.txt 2.txt 3.txt 4.json 5.json
mkdir papka_4 papka_5 papka_6
ls -la
mv 1.txt 2.txt ~/Desktop/choke/papka/papka_2

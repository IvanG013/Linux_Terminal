# Homework | Linux Terminal | part_1
___
___

1. Посмотреть где я

>pwd

2. Создать папку

>Mkdir Itest

3. Зайти в папку

>cd Itest или сd!$ - зайти в созданую папку

4. Создать 3 папки

>mkdir folder_1 folder_2 folder_3 или 

>mkdir -p {folder_1,folder_2,folder_3}

5. Зайти в любоую папку

>cd folder_1

6. Создать 5 файлов (3 txt, 2 json)

>touch app {file_1.txt,file_2.txt,file_3.txt,file_4.json,file_5.json}

7. Создать 3 папки

>mkdir folder_4 folder_5 folder_6

8. Вывести список содержимого папки

>ls folder_1

9.  Открыть любой txt файл

>vim file_1.txt

10. Написать туда что-нибудь, любой текст

>I - для редактирование и пишем текст

11.  Сохранить и выйти

>esc,shift+:,w,q,enter

12. Выйти из папки на уровень выше

>cd ..

13. Переместить любые 2 файла, которые вы создали, в любую другую папку

>mv folder_1/file_1.txt folder_2/file_1.txt

>mv folder_1/file_2.txt folder_2/file_2.txt

14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку

>cp folder_1/file_4.json folder_3/file_4.json

>cp folder_1/file_5.json folder_3/file_5.json

15. Найти файл по имени

> find -iname file_3.txt

16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает.

>tail -f file_1.txt

>ctrl+c выйти с режима

17. Вывести несколько первых строк из текстового файла

>head -4 file_1.txt

18. Вывести несколько последних строк из текстового файла

>tail -4 file_1.txt

19. Посмотреть содержимое длинного файла (команда less) изучите как она работает

>less file_2.txt

>выход q

20. Вывести дату и время

>date

___
___
Задание*

1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request

>Отправил:http://162.55.220.72:5005

>Ответ: Hello!!!!!!!!!
___
___

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

Создаем файл: touch script.sh

Редактируем: vim script.sh

Нажать клавишу "i"

Ввести:

>#!/bin/bash

>cd Itest

>mkdir folder_1 folder_2 folder_3

>cd folder_1

>touch app {file_1.txt,file_2,file_3.txt,file_4.json, file_5.json}

>mkdir folder_4 folder_5 folder_6

>ls -la

>cd ..

>mv folder_1/file_1.txt folder_2/file_1.txt

>mv folder_1/file_2.txt folder_2/file_2.txt


Cохранить и выйти: esc,:,w,q,enter

Выполняем скрипт: ./script.sh 








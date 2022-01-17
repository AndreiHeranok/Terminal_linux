__Задание по терминалу линукс__ - [HW_1](https://github.com/AndreiHeranok/Linux_terminal/blob/main/HW_1.txt)

___

__Linux terminal (GitBash) commands__

1) Посмотреть где я            ```pwd```
2) Создать папку               ```mkdir coursKsendzoff/```
3) Зайти в папку               ```cd coursKsendzoff/```
4) Создать 3 папки             ```mkdir hw_1 hw_2 hw_3```
5) Зайти в любоую папку        ```cd hw_2/```
6) Создать 5 файлов (3 txt, 2 json)     ```touch 1.txt 2.txt 3.txt 4.json 5.json```
7) Создать 3 папки                     ```mkdir h_1 h_2 h_3```
8) Вывести список содержимого папки     ```ls``` 
                                        ```ls -la```     
9) Открыть любой txt файл                    ```vim 1.txt```
10) Написать туда что-нибудь, любой текст.   ```нажать клавишу "i" ввести текст```
                                ```Hello```
                                ```I'm Andrei```
                                ```I'm from Minsk```
11) сохранить и выйти.                 ```"esc" ввести  ":wq"```
12) Выйти из папки на уровень выше            ```cd ..```

13) переместить любые 2 файла, которые вы создали, в любую другую папку.   
```mv 1.txt 2.txt h_1/```
                                                                          
       ```mv 1.txt 2.txt путь к папке/1.txt```  - перенести в другую директорию

14) скопировать любые 2 файла, которые вы создали, в любую другую папку.   ```cp 1txt 2.txt h_1/2.txt``` 
                                                                           
15) Найти файл по имени         ```find . -name 1.txt```
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.  ```tail -f 1.txt``` 
                                                                                       

17) вывести несколько первых строк из текстового файла       ```head -2 1.txt```
18) вывести несколько последних строк из текстового файла    ```tail -2 1.txt```

19) просмотреть содержимое длинного файла (команда less) изучите как она работает.   ```less name_file```
20) вывести дату и время    ```date +"%D %T"```
---
__Задание *__
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000

```curl 'http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000'```

1_1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request

```curl http://162.55.220.72:5005/terminal-hw-request```

приходит ответ с другим заданием.

```curl "http://162.55.220.72:5005/get_method?name=(Andrei)&age=(29)"```

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

Создаём файл: ```touch HW_1_1.sh```

Вносим изменения: ```vim HW_1_1.sh```

нажать клавишу ```"i"``` ввести текст 
```
#!/bin/sh 
cd coursKsendzoff/
mkdir h_1 h_2 h_3
cd h_1/
touch 1.txt 2.txt 3.txt 4.json 5.json
mkdir f_1 f_2 f_3
ls -la
mv 1.txt 2.txt f_1/
```
Cохранить и выйти: ```"esc" ":wq"```

Выполняем скрипт: ```sh HW_1_1.sh``` 
                  ```./HW_1_1 ```

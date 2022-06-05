# 3.1

5. Выделенные ресурсы для виртуальной машины:
   - 1024 Мб оперативной памяти
   - 2 процессора с 100% нагрузкой
   - 64 Гб - жесткий диск
6. Добавить ресурсов:
   - Виртуальной памяти: v.memory = 1024
   - Процессоров: v.cpus = 2
7. Попрактиковался
8. Переменной n можно задать длину вывода журнала. Это описано на 4917-4918 строчках man.
   - Директива ignoreboth соединяет в себе директивы: ignorespace (комманды с пробелом вначале не сохраняются в истории) и ignoredups (в истории не сохраняются последовательно введенные одинаковые комманды).
9. Фигурные скобки используются для перечисления строк. Это необязательный параметр. Например, для создания папок 1,2,3 будет использована команда mkdir {1,2,3}. Описано на 1001 строке  man. 
10. - Создать 100 000 файлов через touch: touch {0..100000}
    - 300000 файлов создать не получится, т.к. команда ограничена в 2048 Кб
11. Конструкция [[ -d /tmp ]] вернет истину, если tmp существует и является каталогом или ложь, если не существует или каталогом не является.
12. - mkdir /tmp/new_path_directory/
    - cp /bin/bash /tmp/new_path_directory/
    - PATH=/tmp/new_path_directory/:$PATH
13. - Комманда at выполняет команды в определенное время
    - Комманда batch выполняет команды в зависимости от уровня загрузки системы

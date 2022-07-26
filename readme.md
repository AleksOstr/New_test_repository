# Что такое Git?

**Git** - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

# Подготовка репозитория

Обычно вы получаете репозиторий Git одним из двух способов:

1. Вы можете взять локальный каталог, который в настоящее время не находится под версионным контролем, и превратить его в репозиторий Git, либо

2. Вы можете клонировать существующий репозиторий Git из любого места.

В обоих случаях вы получите готовый к работе Git репозиторий на вашем компьютере.
Создание репозитория в существующем каталоге

Если у вас уже есть проект в каталоге, который не находится под версионным контролем Git, то для начала нужно перейти в него. Если вы не делали этого раньше, то для разных операционных систем это выглядит по-разному:

для Linux:

    $ cd /home/user/my_project

для macOS:

    $ cd /Users/user/my_project

для Windows:

    $ cd C:/Users/user/my_project

а затем выполните команду:

    $ git init

Эта команда создаёт в текущем каталоге новый подкаталог с именем .git, содержащий все необходимые файлы репозитория — структуру Git репозитория. На этом этапе ваш проект ещё не находится под версионным контролем. Подробное описание файлов, содержащихся в только что созданном вами каталоге .git, приведено в главе Git изнутри

Если вы хотите добавить под версионный контроль существующие файлы (в отличие от пустого каталога), вам стоит добавить их в индекс и осуществить первый коммит изменений. Добиться этого вы сможете запустив команду git add несколько раз, указав индексируемые файлы, а затем выполнив git commit:

    $ git add *.c
    $ git add LICENSE
    $ git commit -m 'Initial project version'

Мы разберем, что делают эти команды чуть позже. Теперь у вас есть Git-репозиторий с отслеживаемыми файлами и начальным коммитом.

# Создание "Сохранений"

Для **добавления измений в коммит** используется команда *git add*. Чтобы использовать команду *git add* напишите 

    git add <имя файла>

Для того, чтобы создать **коммит** (сохранение) необходимо выполнить команду *git commit*. Выполняется она так: 

    git commit -m "<сообщение к коммиту> 
Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

# Переключение между сохранениями

Для переключения между сохранениями используйте команду

    git checkout commit

где commit - это хеш нужного коммита

# Журнал изменений

Чтобы посмотреть журнал изменений, используйте команду

    git log

# Ветки в Git

### **Создание ветки**

Для того, чтобы **создать ветку**, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: 

    git branch <название новой ветки>

# Слияние веток и разрешение конфликтов

Слияние веток

# Удаление веток

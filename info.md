Привет, GitHub и мир
# GIT Instruction

<br>

### Basic commands:
* `git init` - initialize folder;
* `git status` - show the current (текущее) state (состояние) of the file;
* `git add (file name)`- add a file to watch (добавление файла к отслеживанию);
* `git add .` - add all files and folders к отслеживанию в директории/папку;
* `git commit -m "(text commit)"` - add a comment (fix состояния изменений);
* `git log` - выводит all info about the commits с их хеш-кодами;
* `git checkout (..first 4-5 simbol хэш-кода..)` - возвращает файл к выбранному соханению;
* `git checkout (..master\main..)` - return (возврат) the file to the selected (выбранному) save;
* `git diff` - see the difference between the current file and the last (commitувидеть разницу между текущим файлом и последнем коммитом);
* `![..name image..](..link..)` - add images.


### Branch commands:

+ `git branch -m (old_name) (new_name)` - comand for rename branches;
+ `git branch` - show branches in terminal;
+ `git branch (...name_branch...)` - create new branch;
+ `git checkout (..name_branch..)` - transition to another branche;
+ `git branch -d (..name_branch..)` - command to delete branch;
+ `git merge` - command to unite branches.

### GitHub commands: 

- `git push -u (..origin main..)` - протолкнуть local repository в сеть на сервис GitHub или иной. First command при работе с GitHub-ом;
- `git push` - команда для переноса изменений с local repository in remote;
- `git pull` - вытягивает изменения с удаленного репозитория в локальный;
- `git clone (..link..)` - copy remote repository к себе в local приложение.

### +Command to list:
+ `pwd` or `ls` - выводит путь где мы сейчас находимся;
+ `cd ..` - возврат к предыдущей папке по иерархии;
+ `git clone [link] "name repository" COPY` - копирует полностью репозиторий в котором находимся со всеми файлами внутри? Или создает еще один с названием другим?

<br><br>

### Registraton GitHub:
**1.** Go to [GitHub](https://github.com) - remote repository. Service;<br>
**2.** Click on the button **"Sign UP"** to go to the registration window;<br>
**3.** After registretion, make "friends" with the remote repository;<br>
**4.** `Push` the local repository to a remote GitHub. Maybe need avtorization on remote repository;<br>
**5.** Провести изменения с another PC;<br>
**6.** `Pull` relevance condition from remote repository.

<br>

> На семинаре 23.12.22 проходили another variation о подключении к GitHub:
>>+ сначала `clone` пробиваем
>>+ далее уже `push`-им и `pull`-им

<br>

<p align="center">
THE END ....maybe ;)
</p>
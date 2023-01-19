# GIT Guide <br> Инструкция по ГИТ

## Basic <br> Основные команды
|name <br> наименование | description <br> описание |                  
|-----|----|
| **git --version** | print current version GIT <br> печатает текущую установленную версию ГИТ |    
| **git init** | init new local repository <br> инициализирует новый репозиторий|     
| **git status** | get information about current status of repository <br> получить информацию о текущем состоянии репозитория|
| **git add info.md** | add modified file 'info.md' for tracking <br> добавить для отслеживания изменения в файле 'info.md' |
| **git add .** | add all modified files and folders for tracking <br> добавить для отслеживания изменения во всех файлах|
| **git commit -m "comments"** | fix the current status with all changes, comments are required <br> зафиксировать текущее состояние отслеживаемых файлов, с обязательным комментированием |
| **git log** | print history of commits <br> печатает историю фиксаций|
| **git checkout 0000** | go to stage with hash code started with 0000 <br> перейти к состоянию с хэш-кодом 0000 |
| **git checkout master** | go to last committed stage <br> перейти к последнему зафиксированному состоянию|
| **git diff** | print different between current stage and last commit <br> печатает разницу между текущим состоянием файлов и последней фиксацией|

----

## Work with branches <br> Работа с ветвлением

| name <br> наименование | description <br> описание |
|----|----|
| **git branch -m name1 name2** | rename branch from 'name1' to 'name2' <br> переименовывает ветку из 'name1' в 'name2' | 
| **git branch** | print list of branches <br> печатает список существующих ветвей| 
| **git branch new_branch** | create new branch with name 'new_branch' <br> создает новую ветку с именем 'new_branch'| 
| **git checkout name_of_branch** | go to branch with name 'name_of_branch' <br>  переходит на ветку с именем  'name_of_branch' | 
| **git branch -d branch_for_remove** | remove branch with name 'branch_for_remove' <br> удаляет ветку с именем 'branch_for_remove' | 
| **git merge current_branch merged_branch** | merge 'current branch' with 'merged_branch' <br> сливает 'current branch' с 'merged_branch' | 

-----

## Alias  <br> Псевдоним
> Aliases is the most cool feature in GIT. You don't need anymore use long commands names. You can replace them with shortly aliases. <br> Псевдонимы одна из самых крутых фичей ГИТа. Больше нет нужды использовать длинные имена команд, их можно заменить короткими псевдонимами.
> <br> For example: <br> Для примера:

| name <br> наименование | description <br> описание | example  <br> пример|
|----|----|----|
|**git alias.goto checkout** | you can use 'goto' instead to 'checkout' <br> можно использовать  'goto' вместо 'checkout' | *git goto <name_of_branch>*
|**git alias.br branch** | you can use 'br' instead to 'branch' <br> можно использовать  'goto' вместо 'checkout'  | *git br*
|**git alias.st status** | you can use 'st' instead to 'status' <br> можно использовать  'goto' вместо 'checkout'  | *git st*
|**git alias.lo log -- online** | you can use 'lo' instead to 'log --oneline' (-> i love this :-)) <br> можно использовать 'lo' вместо 'log --oneline'  | *git lo*
|**git alias.cm commit** | you can use 'cm' instead to 'commit' <br> можно использовать  'cm' вместо 'commit'  | *git cm -am "comments"*

----

## Beauty log  <br> Привлекательный лог
> A pretty log is a really important part of development, and GIT is no exception. You have a powerful tools that will make your log more readable and beautiful.  <br> Красивый лог по настоящему важная часть разработки, и ГИТ не исключение. В нашем распоряжении есть мощные инструменты для того чтобы сделать лог более читабельным и привлекательным

| command | desc |
|----|----|
|**git log -p -2** | print only last 2 commits  <br> печатает информацию о двух последних фиксациях 
|**git log --oneline** | print log 'one commit -> one line'  <br> печатает информацию 'одна фиксация в- одна строка'
|**git log --graph** | print log with branches graph <br> печатает фиксации с ветками и графическим маркером (ASCI)
|**git log --pretty=format:"%h - %an, %ad : %s"** | formatted print  <br> отформатированная печать

| format | desc |
|----|----|
|**%H** | commit hash code  <br> хэш фиксации 
|**%h** | short commit hash code  <br> короткий хэш фиксации
|**%T** | tree hash code  <br> хэш ветки
|**%t** | short tree hash code  <br> короткий хэш дерево
|**%P** | parent hash code  <br> хэш родительской ветки
|**%p** | short parent hash code  <br> короткий хэш родительской ветки
|**%an** | name of commit author  <br> имя автора фиксации
|**%ae** | email of commit  author  <br> почта автора фиксации
|**%ad** | date when commit was created  <br> дата создания фиксации
|**%cn** | name of version creator  <br> имя создателя ветки
|**%cn** | email of version creator <br> почта создателя ветки
|**%cn** | date when version was created <br> дата создания ветки
|**%s** | comments <br> комментарии

------

## If you make mistake  <br> В случае ошибки

| name <br> наименование | description <br> описание | 
|----|----|
|**git commit --amend** | remove last commit. it will be rewrite with next commit <br> отмена последней фиксации, состояние будет перезаписано при следующей фиксации
|**git reset HEAD filename** | remove last indexed <br> отмена последней индексации
|**git checkout -- filename** | remove all changed after last commit <br> удаление всех изменений в файле после последней фиксации

----

## Remote repository  <br> Удаленный репозиторий

| name <br> наименование | description <br> описание | 
|----|----|
|**git clone** | copy remote repository in local repo <br> копирует удаленный репозиторий в локальный
|**git pull** | get all files from repository <br> получить все что есть в репозитории
|**git push** | pushed all changes in remote <br> отправляет все изменения в удаленный репозиторий 

| | contacts |
|:----|:----:|
| **𝖒𝖎𝖘𝖙𝖊𝖗𝖆𝖇𝖛𝖎𝖗**|  [![My contacts](https://sun6-21.userapi.com/s/v1/if2/0S7UHRKGkZD-lwCxqbHfYmH2JLqnZi3AA1U6b-ZuI13Z8_Zw04x59-6In1tAv3KwQxdb_QUmWwOvj9jBcAmJ4gCT.jpg?size=50x50&quality=96&crop=117,32,256,256&ava=1 "my public social profile")](https://vk.com/misterabvir)[![My contacts](https://sun6-23.userapi.com/s/v1/if1/KeJiiYmL9jFeNvZlRpjEL04jZdsNNA1UjdWln0TdojSedE46q4i2zHwGZB5pY7NZ-JhTSLGr.jpg?size=50x50&quality=96&crop=79,46,410,410&ava=1 "my public contact")](https://t.me/misterabvir)[![My contacts](https://sun6-22.userapi.com/s/v1/ig2/T0-UcGeC5o4VKR3S828eHVzXZRFUMkwt501jwAQoBF4e6cr1Uw-VFioGpNerbBwDFkfe43yWpSnA0kX4VJ83s01j.jpg?size=50x50&quality=95&crop=183,183,655,655&ava=1 "my geekbrains profile")](https://gb.ru/users/8831713)[![My contacts](https://sun6-20.userapi.com/s/v1/ig2/HLuYMTeO-rJPPa9IngY11r1qXLvapXaDWnxglTerVrh5pBGRxtqpP4dLiZQCkxNp4DR4QPKSLMIoFxXPJ07YfPQK.jpg?size=50x50&quality=96&crop=323,55,551,551&ava=1 "my public github repository")](https://github.com/misterabvir)[![My contacts](https://sun6-22.userapi.com/s/v1/if1/_ca-hwLexTXVs_DY72z9CLtRilIyeAmYL8lgqThNhySiW6ynGpmb4lKAKiDq5AxUBPoRHezJ.jpg?size=50x50&quality=96&crop=0,0,200,200&ava=1 "my email")](mailto:abvir@yandex.ru)

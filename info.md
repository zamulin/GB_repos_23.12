# Instruction for work with GIT

## Git main commands

|Command                       | Description           |
|----------------------------- | ----------------------|
|git config --global user.name | sets developer's name |
|git config --global user.email| sets developer's email, that connects to git|

* ***git init*** - initialized of local repository
* ***git status*** - shows current state of the branch from git
* ***git add .*** - command for adding of monitoring of all files
    * *git add info.md* - command for adding a file for its monitoring (in this case info.md)
* ***git commit -m "Comment"*** - fixes state of changes  
* ***git log*** - history of all commits
    1. *git log -p* - provides advanced history of all commits
    2. *git log --graph* - provides history of commits in graphic form
* ***git checkout*** - switch between branches
    * *git checkout master* - checkout to actual state of the file
    + *git checkout branch_name* - chenging your location from master or any other branch into branch_name
* ***git diff*** - to see difference between actual file and the last commit
* ***git branch*** - shows all existing branches
    + *git branch* ***branch_name*** - creates a new branch from the branch where you are in, branch_name - is a name of branch that you would like to create 
+ ***git merge branch_name*** - adds changes from branch_name into your branch where you are in

- ***git pull*** - downloads a copy of the current branch from the specified remote repository and merges it into the local copy
- ***git push origin master*** - sends changes to a remote repository. Specifying the name of the repository and the branch. 
* git branch - provides list of all branches that eist
    * git branch -m old_branch_name new_branch_name
    * git branch new_branch - creates a new branch with name new_branch
 
* git checkout branch_name - swetches one branch to another one 
* git branch -d branch_name - deletes branch with name branch_name

* git merge branch_name - adds chnges from branch_name into current branch

>***git clone*** - clone a repository into a new directory

>***git branch -d branch_name*** - deletes branch with name branch_name

>***git reset*** - is used for cancellation changes
>>***git revert*** - rollsback the last commit. Creates a new commit that contains the reverse transformations relative to the previous one. Adds to the history of the current branch.
>>***git clean*** - is used for removal of garbage from working catalog. Such as project build results or merge conflict files. 

[Useful link to git commands](https://habr.com/ru/company/ruvds/blog/599929/)


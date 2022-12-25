Привет, GitHub и мир

# Instructions for work with Git

## Git general commands:

- git init - initialization of local repository
- git status - get info from git about its actual status
- git clone - retrieve an entire repository from a hosted location via URL
## Git configuration commands:

* git config --global user.name “[firstname]” - set a name that is seen when review version history
* git config --global user.email [valid-email] - set an email address
The commands to be entered only once.
## Git display commands:

- git status - get info from git about its actual status
- git log - displays history of all commits with their #-codes
- git log --oneline - displays history of all commits with their #-codes in short version
- git log --oneline --all - displays history of all commits with changes with their #-codes in short version
- git log --graph - displays all commits with graph tree
- git diff - see difference between actual file and the last commit 
- clear - cleaning of terminal window
## Git commit commands:

- git add [file_name] - command to add one for tracking
- git add . - command to add all files and folders from directory for tracking
- git commit -m "comment" - command to fix status of changes
- git commit -a -m - add commit in one line
- git commit -am - add commit in one line
- git checkout [4 symbols]- move from one commit to other one
## Git branch creation commands

* git branch - displays all branches
* git branch [branch_name] - creation of a new branch
* git checkout [branch_name] - switch between branches
* git checkout -b [branch_name] - create and switch to the new branch
* git merge [branch_name] - merging of branch, to be made when on master branch
* git branch -d [branch_name] - delete branch
* git branch -D [branch_name] - delete already merged branch. BUT: it's impossible to delete a branch while being on it
* git branch -m [old_branch_name] [new_branch_name] - to rename branch
## Git gitignore function:

- .gitignore - create this file and write files names to be ignored. The .gitignore-file itself can be moved inside not to commit it.
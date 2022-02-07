# GIT CHEATSHEET!

## DONT FORGET!
`git commit -S -m "feat(...) : ..."`

## Git Standart
- `git branch <name_branch>` : Create a new branch called `<name_branch>`
- `git branch -d <name_branch>` : Delete the spesified branch (safely)
- `git branch -D <name_branch>` : Delete the spesified branch (forcely)
- `git branch -m <new_name_branch>` : Renaming current branch
- `git branch -a` : List all remote branches


## Git Files
- `git stash save --keep-index --include-untracked` : Delete Change in unstaged files but saving the files.

## Git Rebase
It is used for tidy up your commit order againts to commit order in the base (github remote).

The case is when you make a branch in local, and there is a commit in the base, you should moving forward.

1. First you have to make **Commit** in your local branch.
2. Fetch the remote commit : `git fetch --all`
3. Git rebase : `git rebase origin/develop`
4. Make sure git log is OK. `git log`

## Git undoing commit 
- `git reset --soft HEAD~1` :
- `git push -f origin feat/testing-count-registered-user`

## Git Pulling
When you finish your branch, you cannot merge locally. You should merge it from the base. 

- `git fetch --all`
- `git pull origin develop`


## Setting GPG True
- `git config --global commit.gpgsign true`

## Initialize Condition
- `export DEVELOP=1`
- `export USE_CAPTCHA=1`

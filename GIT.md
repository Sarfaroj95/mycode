## BASIC GIT 13 Sep 2026
```
git clone https://github.com/example.repo/example.git
git status
git add .
git add [file name one by one which file you want to push code]
git branch
git fetch
git switch (branch name - dev)
git commit -m 'commit'
git push -u origin master
git push -u -f bitbucket master
git merge --quit
git commit --amend -m "New commit message"
```
| git CLI  | Description |
|----------|------------|
|git clone | clone any public repo in your local machine|
|git init| initialize git|
|git status | check status for creent any changes|
|git add . | Add all changes file |
|git add README.md | only README.md file add |
|git branch | check current branch |
|git fetch | Update repo |
|git switch dev | switch branch |
|git commit -m "message" | put message |
|git push -u origin master | push code in repo |
|git commit --amend -m "Message"| message|




## GIT STASH & POP

```
git stash
git pull origin QA
git status
git stash -m 'save-code'
git stash pop
git stash list
git stash pop stash@{1}
```
## GIT Granph
```
git log --graph --oneline -10
git log --graph --oneline -all
```

**Pull code from others branch**
> git pull origin main [pull from main branch] <br/>
> git clone https://github.com/Sarfaroj95/angular-unit-test.git

**If you want to clone perticular Branch then**
> git clone -b master https://github.com/Sarfaroj95/angular-unit-test.git

**You can do from your VS Code left side**
   > Click on souce Control <br/>
   > Then click on three dod ... <br/>
   > Stash Scroll below Stash Section -> Any comments <br/>
   > Pop Stash Section -> Pop Latest Stash or Pop Stash with commects

**Basic Part in Git**
   > git config --global --list [Check current user] <br/>
   > git config --global user.name "User" <br/>
   > git config --global user.email "user@example.com"

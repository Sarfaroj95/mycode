## BASIC GIT
```
git clone https://github.com/example.repo/example.git
git status
git add .
git add [file name one by one which file you want to push code]
git branch
git switch (branch name - dev)
git commit -m 'commit'
git push -u origin master
git push -u -f bitbucket master
git commit --amend -m "New commit message"
```

## GIT STASH & POP

```
git stash
git pull origin QA
git status
git stash -m 'save-code'
git stash pop
```

**Pull code from others branch**
> git pull origin main [pull from main branch] <br/>
> git clone https://github.com/Sarfaroj95/angular-unit-test.git

**If you want to clone perticular Branch then**
> git clone -b master https://github.com/Sarfaroj95/angular-unit-test.git

**You can do from your VS Code left side**
   > 1. Click on souce Control 
   > 2. Then click on three dod 
   > 3. Stash Scroll below Stash Section -> Any comments
   > 4. Pop Stash Section -> Pop Latest Stash or Pop Stash with commects

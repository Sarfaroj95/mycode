## GIT
```
git clone https://github.com/example.repo/example.git
git status
git add .
git branch
git switch (branch name - dev)
git commit -m 'commit'
git push -u origin master
git push -u -f bitbucket master
```

## GIT STASH & POP

```
1. git stash
2. git pull origin QA
3. git status
4. git stash -m 'save-code'
5. git stash pop
```

**Pull code from others branch**
> git pull origin main [pull from main branch] <br/>
> git clone https://github.com/Sarfaroj95/angular-unit-test.git

If you want to clone perticular Branch then 
> git clone -b master https://github.com/Sarfaroj95/angular-unit-test.git

> You can do from your VS Code left side
    1. Click on souce Control 
    2. Then click on three dod 
    3. Stash Scroll below Stash Section -> Any comments
    4. Pop Stash Section -> Pop Latest Stash or Pop Stash with commects

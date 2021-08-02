# Change last commit incl. message and files 

```
# Walkthrough 
touch newfile.txt 
git add .
git commit -am "new file added"

# Uups forgotten README 
touch README 
git add .
git commit --amend # README will be in same commit as newfile.txt 
# + you can also changed the commit message 
```

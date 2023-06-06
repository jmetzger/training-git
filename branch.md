# git branch

## Create branch based on commit (also past commit) 

```
git branch lookaround 5f10ca
```

## Delete unmerged branch 

```
git branch -d branchname # does not work in this case 
git branch -D branchname # <- is the solution 
```

## Delete remote tracking branch 

```
git branch -d -r origin/feature/501
```

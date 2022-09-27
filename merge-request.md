# Merge request   
  
```  
# Local 
git checkout -b feature/4822
ls -la
touch f1.txt
git add .
git commit -am "f1.txt"
touch f2.txt
git add .
git commit -am "f2.txt"
git push -u origin feature/4822
```
 
## Online bitbucket / gitlab 
 
```
# create merge request 
# and merge 
```

## Delete branch online after merge 

## Cleanup locally 

```
git fetch --prune
git checkout master
git branch -D feature/4822
git pull --rebase
```


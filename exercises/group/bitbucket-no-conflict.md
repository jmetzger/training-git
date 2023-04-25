# Merge request   
  
## Jeder in der Gruppe erstellt lokal ein Feature   
  
```  
# Local 
# git checkout -b feature/<euer-vorname>
# e.g. git checkout -b feature/jochen1

ls -la
touch jochen1.txt
git add .
git commit -am "jochen1.txt"
git push -u origin feature/jochen1 
```
 
## Online bitbucket / gitlab 
 
```
# create merge request 
# and mergen strukturiert nacheinander 
```

## Delete branch online after merge 

  * eventually done automatically when checkbox was set
  * or: delete from branches menu 

## Cleanup locally 

```
git fetch --prune
git checkout master
git branch -D feature/<euer-vorname>
git pull --rebase
```


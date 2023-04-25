# Merge request with conflict (bitbucket) 
  
```  
# Local 
git checkout -b feature/5021
# ändern zeile1 in todo.txt 
notepad todo.txt 

git add .
git commit -am "aenderung todo.txt"
git push -u origin feature/5021
```

## Online Änderung im master -> todo.txt -> Zeile 1

```
Änderung über web-Oberfläche in bitbucket -> source 
```
  
## Online bitbucket / gitlab 
 
```
# create merge request 
# and merge  --> conflict 
```

## Auflösen des conflicts 

```
git pull origin master 
# lösen den conflict 

git status 

# modfizieren die todo.txt 
notepad todo.txt 

git add todo.txt 
# Konflikt gelöst 
git commit 

# der branche wird nochmal hochgeschoben 
git push 

```

## Merge durchführen 

```
# Wieder in den Pull-Request rein und den Merge durchführen 

```



## Delete branch online after merge 

  * eventually done automatically when checkbox was set
  * or: delete from branches menu 

## Cleanup locally 

```
git fetch --prune
git checkout master
git branch -D feature/5021
git pull --rebase
```


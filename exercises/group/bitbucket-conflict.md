# Merge request mit conflict (Gruppenarbeit) 
 
 ## Phase 1 
 
 
### Jeder in der Gruppe erstellt lokal ein Feature   
  
```  
# Local 
# git checkout -b feature/<euer-vorname>
# e.g. 
git checkout -b feature/jochen2
# Zeile 1 todo.txt 
notepad todo.txt 
git add -A 
git commit -am "todo.txt"
git push -u origin feature/jochen2 
```
 
### Online bitbucket / gitlab 
 
```
# create merge request 
```

## Phase 2


## Online bitbucken - strukturiert mergen 
```
# and mergen strukturiert nacheinander 
# conflict 
```

## Jetzt conflict lokal lösen 

```
# in unserem feature branch
git pull origin master 

# conflict auflösen 
notepad todo.txt 
# entscheiden für codeblock 

# ändern kenntlich machen
git status
git add todo.txt 

# merge ist fertig 
git commit 


git push
```

## Online mergen 

```
## Jetzt dürfte kein Konflikt mehr da sein 
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


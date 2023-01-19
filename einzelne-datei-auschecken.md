# Einzelne Datei auschecken 

## aus anderem Commit 

```
# aus commit 11ed 

git checkout 11ed -- todo.txt
# unterverzeichnis 
git checkout 11ed -- tmp/test.txt 


```

## ...und direkt umbenennen 

```
# datei todo.txt aus 11ae -> Inhalt anzeigen und direkt neue datei umleiten 
git show 11ae:todo.txt > todoneu.txt

# ein commit vorher 
git show 11ae^:todo.txt > todoneu.txt

```

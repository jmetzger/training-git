# setup.sql in SETUP.sql umwandeln (Windows) 

## Problem 

  * Windows erkennt in git keine Änderung der Groß- und Kleinschreibung 
  * Workaround: git rm --cached; git commit -am 

## Walkthrough 

```
touch SETUP.sql 
git add .; git commit -am "SETUP neu" 

# Uups, verschrieben ! Was jetzt ? 
git rm --cached SETUP.sql # Datei wird aus git rausgenommen 
git commit -am "und dingfest machen" 
# Beweis 
git show HEAD # letztes commit mit Änderungen anzeigen 


# Jetzt auf ein Neues 
# oder im Explorer
mv SETUP.sql setup.sql
git add .; git commit -am "setup.sql neu" 
git show HEAD 

```

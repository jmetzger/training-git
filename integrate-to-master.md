# Integrate of files/commits from other commits into master (hotfix) 

## Walkthrough 

```
# 1. Schritt - erstellen integrationsbranch von dev/staging branch
git checkout -b integrate/1

# Möglichkeit 1: cherry-pick - komplette commit inkl. aller Änderungen mit reinnehmen 
# Hier wird gemerged: Gemerged 
# Evtl. Konflikt, den muss ich dann lösen 
git cherry-pick c5906c0

# Möglichkeit 2: Einzelne files aus commit: Achtung, wenn im Work-Directory
# bereits vorhanden überschrieben
# commit wird bereits durchgeführt 
git checkout ddb0 -- armin3.txt

# Möglichkeit 3: cherry-pick ohne commit 
git cherry-pick -n 4497
git status 
# alle files rausnehmen, die wir nicht haben möchten, wie folgt. 
git restore --staged agenda.txt
# Achtung, jetzt sind diese so im Working Directory als unstaged 
# d.h. die alte Version aus dem letzten Commit holen 
git checkout HEAD -- agenda.txt 

# 3. Schritt 
# änderungen commiten
git commit -am "Revised version" 

# 4. Nach online pushed 
git push -u origin integrate/1 

# 5. Merge request in gitlab: integrate/1 -> master 
# und dann mergen online 
```

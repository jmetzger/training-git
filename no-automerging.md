# Prevent automerging 

## Mergen ohne commit, commit selbst nach Überprüfung 

```
git merge --no-commit --no-ff <local-branch>
# schritt 2:
# Entweder. Vergleichen mit diff
# d.h. Index wird verglichen mit letzten Commit
git diff HEAD
# Oder schön mit difftool (wenn konfiguriert) 
git difftool HEAD 
```

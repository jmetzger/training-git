# Mergetools 

## Meld (Windows) - Install  

  *  https://meldmerge.org/

## Find out if mergetool meld is available 

```
# Important: close and reopen git bash before doing that 
# you can try to see, if meld can be executed by simply typing "meld"

git mergetool --tool-help
```

## Configure, when it is found by mergetool --tool-help 

```
# you have to be in a git project 
git config --global merge.tool meld
git config --global diff.tool meld
git config --global mergetool.keepBackup false
git config --list
```

## If not found bei mergetool --tool-help :: Configuration in Git for Windows (git bash) 

```
# you have to be in a git project 
git config --global merge.tool meld
git config --global diff.tool meld
# Should be on Windows 10 
git config --global mergetool.meld.path “/c/Users/Admin/AppData/Local/Programs/Meld/Meld.exe”
# sometimes here 
git config --global mergetool.meld.path "/c/Program Files/Meld/Meld.exe"
# do not create an .orig - file before merge 
git config --global mergetool.keepBackup false
```  

## How to use it 

```
# when you have conflict you can open the mergetool (graphical tool with )
git mergetool
```

# Mergetool tortoisemerge (Windows Only) 

## Step 1: Install tortoisemerge 

  * https://tortoisegit.org/download/

## Step 2: Close git bash if open 

## Step 3: Does git find merge 

```
git mergetool --tool-help
```

## Step 4: Setup tortoisemerge as mergetool 

```
git config --global merge.tool tortoisemerge 
git config --global mergetool.keepBackup false
```

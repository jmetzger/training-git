# git tag 

## Creating tags, Working with tags 

```
# set tag on current commit -> HEAD of branch 
git tag -a v1.0 -m "my message for tag"
# publish 
git push --tags 

# set on specific commit 
git tag -a v0.1 -m "Initial Release" a23c 

# checkout files of a specific tag 
git checkout v0.1 
# or
git checkout tags/v0.1 

```

## git delete tag 

```

# Tag local löschen und danach online löschen 
git tag -d test.tag
git push --delete origin test.tag

# Tag online löschen und danach lokal 
# Schritt 1: Über das interface (web) löschen 
# Schritt 2: aktualisieren 
git fetch --prune --prune-tags 

```

## Misc 

```
# Fetch new tags from online
git fetch --tags 

# Update master branch (rebase) and fetch all tags in addition from online 
git checkout master
git pull --rebase --tags
```

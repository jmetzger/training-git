# Submodules best practice 

## Add submodule 

```
git submodule add https://github.com/jmetzger/training-git.git
```

## Clone repo with submodules (Important !) 

```
git clone --recurse-submodules https://gitlab.com/dummyhoney/jochen111.git training-subtest
```

## Updaten des submodules 

```
git submodule update --remote training-git
git commit -am "new version" 
```

## Best practive 

```
clone repo use for submodule seperately
(in seperate folder)
if you want to change it
```

## Updating commands for updating subfolder 

```
git submodule update --remote 
# use other branch from submodule then master 
git config -f .gitmodules submodule.DbConnector.branch stable
```

## Get rid of submodule 

```
rm -fR training-git/
git rm .gitmodules
git rm training-git
git status
git commit -am "removed submodules"

```


## Ref.

  * https://git-scm.com/book/de/v2/Git-Tools-Submodule

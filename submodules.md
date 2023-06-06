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
# Remove the submodule entry from .git/config
git submodule deinit -f training-git

# Remove the submodule directory from the superproject's .git/modules directory
rm .git/modules/training-git -r -fo

# Remove the entry in .gitmodules and remove the submodule directory located at path/to/submodule
git rm -f training-git
```


## Ref.

  * https://git-scm.com/book/de/v2/Git-Tools-Submodule

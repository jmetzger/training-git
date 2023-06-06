# Submodules best practice 

## Add submodule 

```
git submodule add https://github.com/jmetzger/training-git.git
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

## Ref.

  * https://git-scm.com/book/de/v2/Git-Tools-Submodule

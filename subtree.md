# Using a subtree 

## Prerequisites - Existing local repo 

```
# in der bash 
cd .. 
cp -a training training-neu 
cd training-neu
```


## Walkthrough

```
# -f is needed because commits are different from main project 
git remote add -f training-git https://github.com/jmetzger/training-git.git
git status 
git subtree add --prefix training-git training-git main --squash
```

## Updating 

```
git fetch training-git main
git subtree pull --prefix training-git training-git main --squash
```

## Push 

```
git subtree push --prefix=training-git training-git main
```


## Ref. 

  * https://www.atlassian.com/git/tutorials/git-subtree

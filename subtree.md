# Using a subtree 

## Walkthrough

```
git remote add -f training-git https://github.com/jmetzger/training-git.git
git subtree add --prefix training training-git main --squash
```

## Updating 

```
git fetch training-git main
git subtree pull --prefix training training-git main --squash
```

## Ref. 

  * https://www.atlassian.com/git/tutorials/git-subtree

# git merge 

## Merge without conflict with fast-forward

```
# Disadvantage: No proper history, because only one branch visible in log
# after fast-forward - merge 


# Important that no changes are in master right before merging 
git checkout master
git merge feature/4711

```

## Merge (3-way) also on none-conflict (no conflicts present) 

```
git merge --no-ff feature/4711

```

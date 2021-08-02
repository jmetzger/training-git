# git log 

## Show last x entries 

```
# 
# git log -x 
# Example: show last 2 entries 
git log -2 
```

## Show all branches 

```
git log --all 
# oder wenn alias alias.lg besteht:
# git lg --all 
```

## Show first log entry 

```
# Step 1 - log needs to only show one line per commit 
git log --oneline --reverse 

# Step 2: combine with head 
git log --oneline --reverse | head -1 
```

## Multiple commands with an alias 

```
git config --global alias.sl '!git log --oneline -2 && git status'
```

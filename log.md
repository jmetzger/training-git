# git log 

## Show last x entries 

```
# 
# git log -x 
# Example: show last 2 entries 
git log -2 
```

## Show first log entry 

```
# Step 1 - log needs to only show one line per commit 
git log --oneline --reverse 

# Step 2: combine with head 
git log --oneline --reverse | head -1 
```


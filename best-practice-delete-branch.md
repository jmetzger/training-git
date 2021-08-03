# Delete a branch/branches after merging (pull / merge request) 

```

# After a succesful merge or pull request und gitlab / github
# Follow these steps for a succesful cleanup 

# 1. Delete feature branch in web interface (e.g. gitlab / github)
# e.g. feature/4811 

# 2. Locally on your system prune the remote tracking branch
git fetch --prune 

# 3. Switch to master or main (depending on what you master branch is) 
git checkout master

# 4. Delete local branch 
git branch -d feature/4811

```

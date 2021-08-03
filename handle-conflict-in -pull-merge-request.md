# Handle conflict in pull/merge request 

## Prerequisites 

  * You have a create a branch 
  * you have pushed that branch to github e.g. git pull origin feature/xyz 
  * you cannot merge with github, because you see a conflict 
  
## Conflict why ?

  * You have because the branch you want to into has changes you do not have in branch
  
## How to solve ? 

  * Integrate changes from master into your branch 
  * Push again.
  * Merge, Yeah, Done ! 
  
## Walkthrough

```
# You have conflict in pull request within github
# on your local system with branch
git branch 
* feature/4711
* master

# you fetch the changes online from the branch master 
# and integrate them into.your branch -> feature/4711 
git pull origin master 

# Eventually solve the conflicts now
# the push again 
git push origin feature/4711 

# Now merge the branch within the pull-request menu 


# Delete unneeded feature branch - online 

# Cleanup locally 
git checkout master 
# -D is need because did not integrate branch locally 
git fetch --prune 
git branch -D feature/4711
git pull --rebase origin master 


```

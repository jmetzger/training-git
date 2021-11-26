# Fix conflict in merge request 

## Walkthrough 

```
# create feature-branch and worked on it 
git checkout -b feautre/4711 
# ... changes
git add .; git commit -am "new feature"
# pushed branch online
git push -u origin feature/4711 
# then created merge online 
# feature/4711 --> master 

##### TaDa - It was NOT possible to merge because of conflict 
# unfortunately advice on gitlab/bitbucket is not worth the dime 

# locally, update you feature-branch like so
# NO git pull --rebase please, otherwice, you have to redo you merge_request afterwards 
# get changes from master 
git pull origin master

# fix conflicts 
git add . 
git commit 

# push new version of feature - branch online
git push 

# now you can merge in the merge-request interface on gitlab 

```

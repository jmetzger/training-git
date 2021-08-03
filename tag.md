# git tag 

```
# set tag on current commit -> HEAD of branch 
git tag -a v1.0 -m "my message for tag"
# publish 
git push --tags 

# set on specific commit 
git tag -a v0.1 -m "Initial Release" a23c 

# checkout files of a specific tag 
git checkout v0.1 
# or
git checkout tags/v0.1 

```

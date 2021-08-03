# git push with conflict 

# Failure push 

```
# Step 1: push produces error 
# you have done git push -u origin master the last to setup remote tracking branch by option -u 
git push
Password for 'https://erding2017@bitbucket.org':
To https://bitbucket.org/erding2017/git-remote-jochen.git
 ! [rejected]        master -> master (fetch first)
....
# Step 2: Integrate changes from online 
git pull

# Step 3: Solve conflict 
Auto-merging agenda.txt
CONFLICT (content): Merge conflict in agenda.txt
Automatic merge failed; fix conflicts and then commit the result.
kurs@ubuntu-tr01:~/training$ git status
On branch master
Your branch and 'origin/master' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

# Step 3a: Open file agenda.txt
# Decide for which version 
# - remove all <<<<<< and ====== and >>>>>>>>>>  - lines 

# Step 3b: then: save + exit from editor


# Step 3c: mark resolution
git status
git add todo.txt 

# Step 3d: 
git status
# as written there 
git commit


# Step 4: re-push 
git push 
```

## recipe 

```
git push # failure 
git pull 
git add todo.txt 
git commit 
git push 
```

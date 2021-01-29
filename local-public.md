 # publish local git repo 
 
 ```
 # Step 1: Create repo on server without README and .gitignore /set both to NO when creating
 
 # Step 2: on commandline locally
 cd /path/to/repo
 git remote add origin https://erding2017@bitbucket.org/erding2017/git-remote-jochen.git
 git push -u origin master
 
 # Step 3: for further commits 
 echo "test" > testdatei
 git add .
 git commit -am "added testdatei"
 git push
 ```

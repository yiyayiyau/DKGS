# How to start github with git

1. install git
2. create dir. for example hier **dkgs**
3. find the dir. than right klick and **Git Bash Here** klicken
4. the first time Usage: **git init**
5. find the Url for the remote. for example hier: **https://github.com/yiyayiyau/DKGS.git** (i create the repositore befor)
6. create a remote names dkgs(or other names) for the link. **git remote add dkgs https://github.com/yiyayiyau/DKGS.git**

* Download all file form Url
1. **git pull dkgs master** master is the default branch

* If you modify one file and want upload it. For example "README.md"
1. **git add README.md** to upload this file to local git
2. **git commit -m 'add some informations'**, you write someting to discribtion this modify.
3. **git push dkgs master** It will update this file to default branch. But, it is not comfortable if you direckly change the master brach, if you are not sure it is 100% correct. 

So you need a sub branch. now you can 
1. **git branch b-1.0.0** hier create a branch with branchname b-1.0.0
2. **git checkout b-1.0.0** switch to local b-1.0.0
3. **git add README.md** add file to local b-1.0.0
4. **git commit -m 'add some informations' b-1.0.0** add comments to local b-1.0.0
5. **git push dkgs b-1.0.0** push file to remote b-1.0.0
6. **git checkout master** switch local b-1.0.0 to local master
7. **git merge b-1.0.0** merge it to local master
8. **git push dkgs master** push local master to remote master

other cmds:
**git remote -v** show all remotes
**git branch -a** show all branchs, incl. local and remote branchs, with * is working branch


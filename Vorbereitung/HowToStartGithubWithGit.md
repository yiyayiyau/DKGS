# How to start github with git

1. install git
2. create dir. for example hier **dkgs**
3. find the dir. than right klick and **Git Bash Here** klicken
4. the first time Usage: **git init**
5. find the Url for the remote. for example hier: **https://github.com/yiyayiyau/DKGS.git** (i create the repositore befor)
6. create a remote names dkgs(or other names) for the link. **git remote add dkgs https://github.com/yiyayiyau/DKGS.git**

7. options: load all files from the remote to working dir. **git pull dkgs master** hier master means the master branch
8. if you modify one file in the dir. or you create a new file (or dir.) and want to upload that to the link, for example you modify "README.md", you can **git add README.md** to upload this file to local git
9. than **git commit -m 'add some informations'**, you write someting to discribtion this modify.
10. and than **git push dkgs master** It will update this file to **master** branch. But, it is not comfortable if you direckly change the master brach, if you are not sure it is 100% correct. 

11. so you need a sub branch. now you can **git branch b-1.0.0** hier branchname is b-1.0.0
12. **git checkout b-1.0.0**
13. **git add README.md**
14. **git commit -m 'add some informations'**
15. **git push dkgs b-1.0.0**

Case: you have a old version in your laptop and want update the news from github
1. open Git Bush Here
2. git 
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
//5. **git push dkgs b-1.0.0** 
6. **git checkout master** switch local b-1.0.0 to local master
7. **git merge b-1.0.0** merge it to local master
8. **git push dkgs master** push local master to remote master

other cmds:
**git remote -v** show all remotes
**git branch -a** show all branchs, incl. local and remote branchs, with * is working branch

以下参考自 https://git-scm.com/book/zh/v2/Git-%E5%88%86%E6%94%AF-%E5%88%86%E6%94%AF%E7%9A%84%E6%96%B0%E5%BB%BA%E4%B8%8E%E5%90%88%E5%B9%B6
新建并切换分支iss53
**git checkout -b iss53**
change something
**git commit -a -m 'added a new footer [iss53]'**
来了紧急任务，但iss53还没有修改好
切回master分支，注意保存修改(提交修改)
**git checkout master** 目录切回到分支iss53之前
新建分支hotfix
**git checkout -b hotfix**
完成紧急任务
**git commit -a -m 'fixed xx'**
合并hotfix到master
**git checkout master**
**git merge hotfix**
删除hotfix分支
**git branch -d hotfix**
切换到iss53继续该任务
**git checkout iss53**
完成该任务
**git commit -a -m 'finished the new footer[iss53]'**
将该工作合并到master
**git checkout master**
**git merge iss53**
删除iss53
**git branch -d iss53**

如果在两个不同的分支中修改了同一部分，则在合并的时候会产生冲突
此时git做了合并但并没有自动创建一个新的合并提交。在你合并冲突后使用
**git status**查看因冲突而未合并的文件
可选 手动修改 或 **git mergetool**
最后
**git commit -a -m ...**




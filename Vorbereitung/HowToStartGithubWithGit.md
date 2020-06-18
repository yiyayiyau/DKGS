# How to start github with git and start group working

## For first Usage: step 1 Install and fork the reponsitory

1. create a Github contour
2. install git(https://git-scm.com/downloads), if you correctly installed, use **git --version** in your **cmd**, you will get version 		of your git
3. Open our group reponsitory webside:  https://github.com/yiyayiyau/DKGS
4. In the mitte top-right find and click **"Fork"** and wait a few second, you will find this reponsitory in your reponsitoriers.

## For first Usage: step 2 Copy the reponsitory to your laptop

1. create a directory in your laptop, for example hier names **dkgs**
2. and than right klick and **Git Bash Here** klicken. (it will open a window and names "WINGW64:/...", this is the git-cmd-windows.)
3. **git init** 
4. Open your Github in your repositories find **https://github.com/xxxxxx/DKGS** and klick it. (xxxxxx is your profile name) In the right bottom, the green butten 	**Clone or download** find the adress: **https://github.com/xxxxxx/DKGS.git**, remember the adress.
5. **git remote add dkgs https://github.com/xxxxxx/DKGS.git** (run this code in your git-cmd-windows, it will create a remote names 	dkgs(you can also write another name instead it) for your dkgs repository. It might ask you to connect with your Github account, 	please follow it.)
6. **git pull dkgs master** (copie alle files from your dkgs reponsitory)

Until now, you have all the same file with the others. Now, image that you have changed some code in anyone file or create a new file. Anyway, you changed some file. You want to share with us. You should:

## Steps to share the changes with us

1. In your laptop find the the directory **dkgs** and right click **"Git Bush hier"**
2. **git pull dkgs master** (look wheather others have changed the same file or same line with your, if yes, it will show it and allow 		you to change it again)
2. **git add test.txt** (find the changed file test.txt, you might need **cd xxxaFileDirectoryName** or **ls** to list all the files 	in the directory)
3. **git commit "add say hello command or some discrebtion information"** (give some information about changes)
4. **git push dkgs master** (push it to your remote)
5. Now, if you open you GitHub you will find the changed file test.txt is in your Github dkgs reponsitory. Click in the mittle left 	button "new pull request" and "Create pull Request"
6. Than i will get the pull request and i will check it and add some discribtion about it. If i merge it, it will be added in my 		repository and next time if someone **pull** the reponsitory, he will also get the changed file.

## Create neu Pull Request OR Update Fork 
### Create neu Pull Request: If you want upload your changes to Upstream
1. Opem Github and find the Fork Repo.
2. Under "Code" click "Neu pull Request"
3. Check "base repository" is "yiyayiyau/DKGS" and "head repository" is your Fork. (default)
4. Click "Create pull request" and give update informations so that in the feature you will not forget what you have done.


### Update Fork: If other teammate something updates and you want get the neuest Fork
1. Open Github and find the Fork Repo.
2. Under "Code" click "Neu pull Request"
3. Check "base repository" is your Fork und "head repository" is "yiyayiyau/DKGS" (This is different with "Create neu Pull Request")
4. Click "Create pull request"
5. Click "merge pull request"
Until now, you can try on it and hopefully everything is ok for you.

## Other with git 
### Create neu Pull Request
1. **git request-pull -p master yiyayiyau master** -p options, meaning show changes

https://git-scm.com/docs/git-request-pull

--Done

The Upstream can with the commands merge the Request.
1. git remote add Immo https://....
2. git fetch Immo master
3. git diff master Immo/master
4. git merge Immo/master
5. git push

### Update Fork
1. **git remote -v"** Check weather yiyayiyau-remote av..
If you don't have any romote with this Link https://github.com/yiyayiyau/DKGS.git , than use:
	* **git add yiyayiyau https://github.com/yiyayiyau/DKGS.git** 
2. **git pull yiyayiyau master** update und merge in your local. This is the same as : *git fetch yiyayiyau*  and  *git merge yiyayiyau/master* together.
3. **git pull dkgs master** dkgs is a remote name, if you have another name, just instatt. 
4. **git push** update und merge in your remote repository.



https://zhuanlan.zhihu.com/p/37281534

https://blog.csdn.net/sunny_happy08/article/details/81078163?utm_medium=distribute.pc_relevant.none-task-blog-baidujs-1

In Gerneral hier is the moster useful commands right now:
1. **git pull dkgs master**
2. **git add xxxx.md** 
3. **git commit -m 'add some informations'**
4. **git push dkgs master** 
5. new pull request in Github
Use **git add ...** you can add files and directory also.





## additional, add sub branch

So you need a sub branch. You can 
1. **git branch b-1.0.0** hier create a branch with branchname b-1.0.0
2. **git checkout b-1.0.0** switch to local b-1.0.0
3. **git add xxxx.md** add file to local b-1.0.0
4. **git commit -m 'add some informations' b-1.0.0** add comments to local b-1.0.0
5. **git push dkgs b-1.0.0** 
6. **git checkout master** switch local b-1.0.0 to local master
7. **git pull dkgs master** compare with remote master
	if faild, changes files and **git add ...git commit... git pull** again
8. **git merge b-1.0.0** merge it to local master
9. **git push dkgs master** push local master to remote master


## other cmds:
**git remote -v** show all remotes
**git branch -a** show all branchs, incl. local and remote branchs, with * is working branch

## some reference and Uncertain code, please ignore it 

[参考](https://segmentfault.com/q/1010000009549291)

[以下参考自](https://git-scm.com/book/zh/v2/Git-%E5%88%86%E6%94%AF-%E5%88%86%E6%94%AF%E7%9A%84%E6%96%B0%E5%BB%BA%E4%B8%8E%E5%90%88%E5%B9%B6)
1. 新建并切换分支iss53
	**git checkout -b iss53**
2. change something
3. 提交
	**git commit -a -m 'added a new footer [iss53]'**
4. 来了紧急任务，但iss53还没有修改好
5. 切回master分支，注意保存修改(提交修改)
	**git checkout master** 目录切回到分支iss53之前
6. 新建分支hotfix
	**git checkout -b hotfix**
7. 完成紧急任务
8. 提交
	**git commit -a -m 'fixed xx'**
9. 合并hotfix到master
	**git checkout master**
	**git merge hotfix**
10. 删除hotfix分支
	**git branch -d hotfix**
11. 切换到iss53继续该任务
	**git checkout iss53**
12. 完成该任务，并提交
	**git commit -a -m 'finished the new footer[iss53]'**
13. 将该工作合并到master
	**git checkout master**
	**git merge iss53**
14. 删除iss53
	**git branch -d iss53**

如果在两个不同的分支中修改了同一部分，则在合并的时候会产生冲突
	此时git做了合并但并没有自动创建一个新的合并提交。在你合并冲突后使用
	**git status**查看因冲突而未合并的文件
	可选 手动修改 或 **git mergetool**
	最后
	**git commit -a -m ...**

https://backlog.com/git-tutorial/cn/stepup/stepup2_7.html

删除文件 **git rm xxxx**
移动文件 **git mv file.txt Vorbereitung/file.txt**
解决冲突需要的命令 
* git status
* git stash
* git stash apply
返回以前版本需要的命令
* git log
* git reflog
* git reset --hard xxxx
查看所有文件
git ls-files
git add -u 自动找到修改的地方

https://git-scm.com/book/zh/v2

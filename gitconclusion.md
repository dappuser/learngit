#git主要技巧自我归纳
###库操作
创建空目录 $ mkdir 库名

添加库 $ git init
###文件操作
添加编辑文件 $ gedit 文件名.

添加文件到暂存区/工作区 $ git add 文件名.

添加文件到版本库 $ git commit -m"版本名"

显示库状态变化 $ git status

查看文件内容 $ cat 文件名.

丢弃工作区的修改并恢复到版本库的版本 $ git checkout -- 文件名.

撤销工作去的修改 $ git reset HEAD 文件名.

删除工作区的的文件 $ git rm 文件名.
###githup传输
远程库与本地库连接 $ git remote add origin git@github.com:（githup账户名）/learngit.git

本地库的所有内容推送到远程库上 $ git push -u origin master（第一次）
                           $ git push origin master（往后）
                           
远程库克隆 $ git clone git@github.com:（githup账户名）/库名.git 

查看远程库信息 $ git remote 

远程上传至分支 $ git push origin 本地分支名：远程分支名

##远程合并方法
从远程的origin仓库的master分支下载代码到本地的  $ git fetch origin master

比较本地库与远程库的区别 $ git log -p master.. origin/master

合并远\本两库 $ git merge origin/master

撤销合并 $ git merge --abort 

从远程的origin仓库的master分支下载到本地并新建一个分支  $ git fetch origin master:分支名

查看本地与分支区别 $ git diff 分支名  之后合并


###分支
创建并转到分支 $ git checkout -b 分支名

查看当前分支 $ git branch

切回总分支 $ git checkout master

合并分支内容至总分支 $ git merge 分支名

删除分支 $ git branch -d 分支名  ||强制删除分支 $ git branch -D 分支名

查看分支合并图 $ git log --graph

保存工作现场 $ git stash 回到现场 $ git stash pop
 
给分支打标签 $ git tag 标签名
                    
$ sudo lsof -i:端口号 查占用的pid号   $ sudo kill -9 pid号 切掉进程

导入新angular项目 sudo npm install --unsafe-perm -g polymer-cli

配置用户名和邮箱

git config --global user.name "yyt"

git config --global user.email "2997353803@qq.com"

上传文件两部

git add ./readme.md

git commit -m "说明"

git add ./

git commit --all -m （提交全部）

查看当前状态

git status

查看日志

git log

git log --oneline

回退

git reset --hard Head~0 (可接0 1 2 3 ...)

git reset --hard Head [版本号]   （版本号通过git log --oneline可查询）

查看之前所有的状态

git reflog





分支 （平行宇宙） master和dev两个仓库  master是主分支

1.创建分支(刚创建的分支和master里的东西是一样的)

git branch dev (创建分支dev)

git branch（可以查看当前有哪些分支 *dev代表当前的分支）

2.进入分支

git checkout dev (进入分支dev)

3.分支中对代码进行操作

git add ./ git commit -m "操作"（操作分支）

4.退出分支 进入到master

git checkout master

5.对两个分支进行合并

git merge dev(将dev分支红修改的内容加到了主分支master中)

git branch -d dev(删除dev分支)





上传文件

git push https://github.com/yyt123456/first-test.git master

拿文件

git pull https://github.com/yyt123456/first-test.git master(需要现在本地初始化一个git仓库)

git clone https://github.com/yyt123456/first-test.git  (不需要初始化 直接拿所有文件)



ssh方式上传 

ssh-keygen -t rsa -C "2997353803@qq.com"

git pull git@github.com:yyt123456/first-test.git master(ssh地址取文件)



先pull在push拿到最新的文件

git pull https://github.com/yyt123456/first-test.git master（如果感觉总写中间的地址麻烦 可以先定义一个变量如下）

git remote add origin https://github.com/yyt123456/first-test.git

然后执行拿或者上传代码的命令

git push origin master/ git pull origin master

git push origin -u master（做了一个远程关联 下次取数据直接用下面命令）

git push/git pull










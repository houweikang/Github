# Github
#注册
git config --global user.name "name"
git config --global user.email "name"

#创建新目录
$ mkdir learngit

#当前目录
$ cd learngit
显示当前目录
$ pwd
/Users/michael/learngit

#文件列表
$ ls

#将当前目录变成Git可以管理的仓库
$ git init
Initialized empty Git repository in /Users/michael/learngit/.git/

#千万不要使用Windows自带的记事本编辑任何文本文件

#文件添加到仓库
$ git add readme.txt

#用命令git commit告诉Git，把文件提交到仓库,m后面是本次提交的说明，commit可提交多个文件
$ git commit -m "message"

#查看结果
$ git status

#查看不同
$ git diff readme.txt

#查看历史记录
$ git log
#美化
$ git log --pretty=oneline

#退回上个版本
$ git reset --hard HEAD^
#退回1094a版本
$ git reset --hard 1094a

#查看文件
$ cat readme.txt

#查看操作命令记录
$ git reflog

#上传本地库到github
$ git remote add origin git@github.com:houweikang/Gittest.git
#第一次删除
$ git push -u origin master
#之后上传
$ git push origin master

#克隆github远程库到本地库
$ git clone git@github.com:houweikang/Github.git

#创建dev分支，切换到dev分支
$ git checkout -b dev
#相当于
#创建dev分支
$ git branch dev
#切换到dev分支
$ git checkout dev

#查看当前分支
$ git branch

#合并分支
#先切换分支
$ git checkout master
#合并分支
$ git merge dev

#查看分支合并图
$ git log --graph

#删除分支
$ git branch -d dev

test --on-ff


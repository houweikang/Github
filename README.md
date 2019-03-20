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

---
title: github快捷键
date: 2019-02-06 22:00:28
tags: 常用软件快捷键
---

- git status 查看状态
- git pull从远程仓库拿下来
- rm ###.###删除
- git rm ###.###从版本库删除该文件并git commit
- cd D:某个位置
- git init 初始化
- git diff 文件名：查看上次修改了什么内容
- git log查看不同版本
- git log --pretty=oneline精简
- git add 文件名
- git commit -m"备注做了什么事情"
- git reset --hard HEAD~1..100,回退前几个版本。HEAD^上一个版本，HEAD^^上上个版本；；既可以回退版本，也可以把暂存区的修改回退到工作区。当我们用HEAD时，表示最新的版本
- git reset --hard （commit id的前五个）：就可以到回退的版本
- git reflog 记录了每一次的命令
- git checkout -- 文件名 :回到最近一次commit或add时的状态
- rm file 删除某个文件，在当前版本库中
- git rm file确实从版本库删除
- git push origin matser把本地的master分支最近修改推送至GitHub
- git remote add origin git@github.com:DarlingCake/(本地名字).git关联远程库，然后再git push -u origin master.其中-u第一次不仅远程，还可以关联，对以后简化命令
- git clone git@github.com:DarlingCake/(repositoriesName).git克隆本地库
- git checkout -b <name>。加-b参数表示创建并且换可以看做git branch 分支名，再git checkout 分支名。
- git branch查看当前分支
- git checkout <name>：切换分支
- git merge <name>：用于合并指定分支到当前分支。
- git branch -d <name>，delete吗，就是删除分支
- git log --graph --pretty=oneline --abbrev-commit,看看分支历史
- git stash把当前的工作现场储存起来
- git stash list查看刚才工作现场存哪了
- git stash apply恢复现场，但stash不删除，需要git stash drop删除
- 另一种git stash pop恢复的同时删除stash
- git stash apply stash@{number}而多次stash，恢复用这个恢复指定的stash
- git remote：查看远程仓库的信息，git remote -v,查看更详细的内容
- git push origin master推送整个分支
- git push origin <name>推送分支
- git tag <name>可以打一个新标签，先切换到需要打标签的分支上
- git tag 查看所有的标签
- git tag -d <tagname>则是删除标签
- git tag <tagname> <commit id>对某次commit打标签，则是对对应的commit id进行打标签
- git show <tagname>可以查看标签信息，标签按字母排序
- git tag -a <tagname> -m"说明文字" <commit id>这样可以创建带有说明的标签，再用上一个，可以看说明文字
- git push origin <tagname>推送标签到远程git push origin --tags一次性全部推
- git push origin :refs/tags/<tagname>远程删除标签

要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；

关联后，使用命令git push -u origin master第一次推送master分支的所有内容；

此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；

分布式版本系统的最大好处之一是在本地工作完全不需要考虑远程库的存在，也就是有没有联网都可以正常工作


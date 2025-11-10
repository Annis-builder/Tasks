# Git提交练习文档  

## 一.查看当前远程仓库配置  

` git remote -v` 

  1.已关联   

`origin  https://github.com/你的用户名/仓库名.git (fetch) `

`	origin  https://github.com/你的用户名/仓库名.git (push)`

2.未关联  

`	fatal: not a git repository (or any of the parent directories): .git`  

   (1)初始化  

​	`git init`  

   (2)添加关联

​	`git remote add origin https://github.com/你的用户名/仓库名.git`  

   (3)验证   

​	`git remote -v git status`   

​	这个时候会有蓝绿色的(master)

## 二.提交文件   

1.检查当前状态  

`git status`  

2.添加要提交的文件  

`git add 文件名//提交单个文件  `

`git add .//提交所有修改的文件`   

`git add -A//提交所有文件`  

3.检查当前状态  

`git status`//如果文件变为绿色,则已添加到暂存区   

4.提交到本地仓库 

`//简单的提交信息 `

`git commit -m "你的提交说明" `

`//详细的提交信息示例 `

`git commit -m "添加新功能：用户登录模块"`  

5.推送到远程仓库

`//如果是第一次推送 git push -u origin main `

`//或者（取决于分支名） `

`git push -u origin master `

`//之后的推送可以简化为 `

`git push`  







   


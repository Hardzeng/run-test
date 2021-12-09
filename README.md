# Github新手使用指南

## 将本地文件上传至Github仓库流程

1. 创建新文件夹、打开  

   ```
   cd name   ##进入XX文件夹
   ```

2. 初始化文件夹

   ```
   git init   ##初始化文件夹
   ```

3.  本地添加提交至GitHub

   - 提出更改（添加至暂存区）

     ```
     git add <filename>   ##添加至暂存区
     or
     git add *
     ```

   - 提交改动（添加至HEAD）

     ``` 
     git commit -m "代码提交信息"   ##备注修改内容，记录作用
     ```

   - 推送至GitHub仓库

     ```
     git push origin master   ##推送至master分支，可以修改为其他分支
     ```

     若将仓库添加至某个远程服务器

     ```
     git remote add origin <server>
     ```

## Git 本地仓库工作流程

working →   index  →  head

![](trees.png)

## 上传
1. $ git add README.md                         # 添加文件  
2. $ git commit -m "添加 README.md 文件"        # 提交并备注信息
3. 提交到 Github
+ $ git remote add origin git@github.com:tianqixin/runoob-git-test.git
+ $ git push -u origin master

## 仓库同步本地
1. $ git fetch origin
2. $ git merge origin/master


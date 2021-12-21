# GitHub新手使用指南

## Git本地仓库工作流程

- ###### 本地仓库由Git 维护的三棵“树”组成。

- ###### 第一个是你的**工作目录（Working Dir）**，它持有实际文件；

- ###### 第二个是**暂存区（Index Stage）**，它像个缓存区域，临时保存你的改动；

- ###### 第三个是**HEAD**，它指向你最后一次提交的结果；

![image-20211221195204215](../AppData/Roaming/Typora/typora-user-images/image-20211221195204215.png)

## Git 分支工作流程

- ###### 分支是用来将特性开发绝缘开来的；

- ###### 在创建仓库的时候，*master* 是“默认的”分支；

- ###### 在其他分支上进行开发，完成后再将它们合并到主分支上；

![image-20211221195330895](../AppData/Roaming/Typora/typora-user-images/image-20211221195330895.png)

## 将本地文件上传至GitHub仓库流程

###### 创建新文件夹、打开

```
cd name   ##进入XX文件夹
```

###### 初始化文件夹

```
git init   ##初始化文件夹
```

###### 本地添加提交至GitHub

- ###### 提出更改（添加至暂存区）

  ```
  git add <filename>   ##添加至暂存区
  or
  git add *
  ```

- ###### 提交改动（添加至HEAD）

  ``` 
  git commit -m "代码提交信息"   ##备注修改内容，记录作用
  ```

- ###### 推送至GitHub仓库

  ```
  git push origin master   ##推送至master分支，可以修改为其他分支
  ```


- ###### 若将仓库添加至某个远程服务器

  ```
  git remote add origin <server>
  ```

###### 分支改动

- 创建"feature_x"分支，切换过去：

  ```
  git checkout -b feature_x
  ```

- 切换回主分支：

  ```
  git checkout master
  ```

- 把新建的分支删掉：

  ```
  git branch -d feature_x
  ```



## 上传

1. $ git add README.md               # 添加文件  
2. $ git commit -m "添加 README.md 文件"        # 提交并备注信息
3. 提交到 GitHub
+ $ git remote add origin git@github.com:tianqixin/runoob-git-test.git
+ $ git push -u origin master

## 仓库同步本地
1. $ git fetch origin
2. $ git merge origin/master


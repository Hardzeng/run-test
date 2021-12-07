# test
### 测试 git fetch、git merge
## 上传
1. $ git add README.md                         # 添加文件
2. $ git commit -m "添加 README.md 文件"        # 提交并备注信息
3. 提交到 Github
+ $ git remote add origin git@github.com:tianqixin/runoob-git-test.git
+ $ git push -u origin master

## 仓库同步本地
1. $ git fetch origin
2. $ git merge origin/master

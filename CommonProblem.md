## GitHub 新手使用指南-常见问题

1. #### 图片不显示

   在上传文章至GitHub时，带有图片的文章会出现如下图片无法显示的情况：

   ![](images/picture problem.png)

   **解决办法**：

   - 新建一个`images`图片文件夹至本地仓库中

   ![](images/picture1.png)

   - 在文章中插入图片时使用相对路径

     ```
     /images/pictures.png
     ```

   - 将`images`文件夹`Push`至GitHub仓库

     ```
     git init   #初始化文件夹
     
     git add images  #增加images文件夹，将内容写入暂存区
     
     git commit -m "add some pictures"  #提交暂存区到本地仓库
     
     git push origin master /git push origin master:master  #将本地master分支推送到origin主机的master分支
     ```

   - 然后将文章上传至GitHub中，图片就可以正常显示了。

2. ####  若服务器端修改文章内容，本地push文章会报错

   ![rejected error](images/error-rejected.png)

   **原因：**由于在GitHub网站上编辑了README文件，本体与网站内容不一致

   **解决办法**：提交之前先更新本地内容

   ```
   git pull
   ```

3.  

8. 
#### GIT 常用操作

1. ##### 提交

   ##### git commit

2. ##### 创建分支

   ##### git branch 分支名字

3. ##### 切换分支

   ##### git checkout 分支名字

4. ##### 创建并切换

   ##### git checkout -b 分支名字

5. ##### 合并分支

   ##### git merge 分支名字(将分支合并到当前分支)

6. ##### 将当前分支设为最新分支

   ##### git rebase 分支名字

7. ##### 撤销变更

   - ##### git reset	（本地，参数是前一个提交）

   - ##### git revert       （远程，参数是当前提交)

8. ##### 选择分支

   ##### git cherry-pick 提交名字

9. ##### 修改用户名密码

1. 用户名和邮箱地址的作用

   用户名和邮箱地址是本地git客户端的一个变量，不随git库而改变。

   每次commit都会用用户名和邮箱纪录。

   github的contributions统计就是按邮箱来统计的。

2. 修改密码

   git config --global credential.helper store (输入这个命令后,以后只要在输入一次用户名密码)

3. 查看用户名和邮箱地址：

   ```
   $ git config user.name
   $ git config user.email
   ```

4. 修改用户名和邮箱地址：

```
$ git config --global user.name "username"
$ git config --global user.email "email"
```

14.检出单个文件

​	git checkout --patch 分支名 文件路径

​	git checkout -- patch master server/src/mod/mod_main_task.erl


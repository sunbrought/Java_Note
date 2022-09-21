## git基本命令的简单使用

1. 初始化git仓库（工作区）

```shell
git init
```

2. 保存到暂存区

```shell
git add .
```

3. 提交到本地仓库

```shell
git commit -m "init commit"
```

4. 关联远端仓库

```shell
#关联远端
git remote add origin
#关联一个远程库时必须给远程库指定一个名字，origin是默认习惯命名
git remote add origin git@gitee.com:veritable/renren-fast-vue.git
#查看本地仓库与远端是否关联
git remote -v 
```

5. 查看本地仓库分支，状态

```shell
#查看本地分支
git branch
#查看远端分支
git branch -r
#查看本地仓库状态
git status
#查看本地和远端仓库
git branch -a
#切换分支
git checkout master
#合并分支(切换到主分支操作)
git merge dev
```

6. 推送到远端仓库

```shell
#推送到远端仓库
git push -u origin master
#本地与远端仓库不一致强制推送(第一次推送)、
git push -u origin master -f
#第一次推送的时候需要 -u 或者 -r 命令,以后可直接进行更新、提交、推送操作。
```

7. 更新代码

```shell
git pull 
#文件路径 ––查看该文件与上次提交修改代码的差别
git diff
#显示提交的日志
git log
#合并临时分支到当前分支
git cherry-pick temp
```

附：git配置提交用户信息

```shell
$ git config --global user.name "***"  #名称
$ git config --global user.email ****@qq.com   #邮箱
```




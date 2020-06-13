### 仓库创建

```git init```

### 版本创建

```git add file```

```git commit -m '描述信息'```

.git版本库里面有暂存区,git add提交到暂存区

git commit创建版本记录,可以多次add,一次性提交



### 版本查看

```git log```

```git log --pretty=oneline```

### 版本回退

```git reset --hard HEAD^^||版本号```    (head-1,head-100 向后面版本)

```git reflog```查看之前创建的记录得到序列号



******

```git status```查看工作区

### 撤回修改

```git  checkout -- file```

 

### 对比文件

```git diff HEAD  HEAD^ -- file```

### 删除文件

```rm file```

**********

### 仓库交互

点击github的settings,有个SSH.

生成电脑ssh公样:  

```git config --global user.name ="邮箱"```

```git config --global user.email ="邮箱"```

```ssh-keygen -t rsa(加密方式) -C '邮箱'```



文件生成到 /home/fu/.ssh/id_rsa

文件有 id_rsa(私钥),id_rsa.pub(ssh公钥),known_hosts

```cat id_rsa.pub```

加到github

### 克隆

```git clone ssh```

克隆出错:

```eval "$(ssh-agent -s)"```

```ssh-add```

### 分支

```git checkout -b 名字```

本地分支跟踪远程的分支:

```git branch --set-upstream-to=origin/分支名 分支名```

删除分支:

```git branch -d 分支名```

### 关联github仓库

```git remote add origin ssh```



### 推送

```git push (-u) origin(远程的分支)  master```



### 拉取代码

```git pull origin 分支名```





### 工作使用git

1. 项目经理搭建框架

2. 员工生成ssh公钥,提交项目经理,经理添加到服务器

3.  克隆,创建提交分支

   Master:保存发布的项目代码

   Dev:保存开发过程中的代码
##### 1. W: Failed to fetch http://packages.microsoft.com/repos/vscode/dists/stable/InRelease  Temporary failure resolving 'packages.microsoft.com'

解决方法:

```
cd /etc/apt/sources.list.d
sudo rm ./vscode.list   (google-chrome.list\)
sudo apt-get update
```

##### 2.换源

**地址:  https://blog.csdn.net/YooLcx/article/details/104527734**

deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal main restricted
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal-updates main restricted
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal universe
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal-updates universe
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal multiverse
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal-updates multiverse
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal-backports main restricted universe multiverse
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal-security main restricted
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal-security universe
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu/ focal-security multiverse

##### 3.Django安装和创建

```
sudo apt install python3-pip
sudo pip3 install Django
python3 -m django --version

//创建
django-admin startproject 项目名
```

##### 4.主题更换

[gnome-look.org]()

/usr/share/themes

##### 5.软件商店透明问题

```sudo apt install gnome-software```



### 6.failed to fetch

```sudo vim /etc/resolv.conf```

修改nameserver为8.8.8.8
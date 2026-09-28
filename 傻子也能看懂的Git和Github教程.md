# Git和Github简介
>Git---本地代码仓库
Github---云端代码仓库
## Git下载与安装
点击此处下载Git：[下载连接](https://git-scm.com/install/windows)
### 1.根据自己的系统选择下载链接(这里以Windows系统为例)
![image](./images/2-1image.png)
#### 注：下载较慢可使用阿里镜像下载:[下载链接](https://registry.npmmirror.com/binary.html?path=git-for-windows/)
### 2.按照如下步骤操作安装即可
***注：除了下面提到的特殊步骤之外其余均选择默认即可，无需更改***
![image](./images/2-2-1.png)
***这一步需将Additional icons选上***
![image](./images/2-2-2.png)
***这一步是将VsCode设为默认的编辑器(后面连接Github等操作均在Vscode上进行)***(VScode怎么安装？请移步其他教程喵！)
![image](./images/2-2-3.png)
***将默认分支名字改为main***
![image](./images/2-2-4.png)
![image](./images/2-2-5.png)
![image](./images/2-2-6.png)
![image](./images/2-2-7.png)
![image](./images/2-2-8.png)
![image](./images/2-2-9.png)
![image](./images/2-2-10.png)
安装完 Git 之后，要做的第一件事就是设置你的用户名和邮件地址。 这一点很重要，所以此时需要用到Github账号，接下来本文将进行GitHub的安装与注册教程

>git config --global user.name "John Doe"  
>git config --global user.email johndoe@example.com

## Github下载与注册
### 1.加速器下载
由于访问GitHub网站不稳定需要用到加速器，这里推荐一款加速器:[下载链接](https://steampp.net/)
1.建议使用微软商店下载,如下图所示
![image](./images/2-3.png)
2.打开应用对GitHub进行加速
![image](./images/2-4.png)
3.打开GitHub官网,网址如下：[GitHub官网](https://github.com/)
如果有GitHub账号点击登录：sign in
没有Github账号点击注册:sign up
![image](./images/2-5.png)
>注：1.Email可以使用QQ邮箱(我用的就是喵~)因为到时候收取验证码的时候方便，***一定要记住！***
2.Password不要忘记哈！
3.Username自己起，尽量用英文，自己给自己起个英文名字不简简单单，实在不行网上搜一个！***一定要记住！***
4.地区选HongKong，我就这样选的
5.还有一些额外的，不得不说一下，注册的时候***不要用校园网***(不要问我怎么知道的)，据说用***手机注册成功率更高***，我用电脑没注册上，用手机注册上了

![image](./images/2-6.png)
4.来到这个界面，恭喜你，注册成功了！
![image](./images/2-7.png)
## 验证Git是否安装成功
### 方法一：打开Vscode,左边配置发生变化说明Git安装成功
![imagee](./images/3-1.png)
### 方法二：win + R 打开cmd输入该命令：git --version，显示git版本说明安装成功
## 设置用户名和邮箱
还记得在Git安装的最后要设置自己的用户名和邮箱吗？
***现在打开Vscode，点击终端，将刚才那两条命令输进去***
以防你不记得那两条命令是啥？
>git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
***这里的用户名就是刚刚注册Github时你自己起的，邮箱也是你自己的，不要告诉我你给忘了吧！***
# Git本地提交和Github远程提交
## Git本地提交
1. 在电脑桌面上创建一个文件夹(此处命名为git-ceshi)
2. 打开Vscode，将该文件夹托入,新建文件，文件类型自定义(.py,.html等等),将代码编辑好后Ctrl + s保存
3. 点击SOURCE CONTROL(源代码管理)，再点击Initialize Repository(初始化仓库)
4. 为此次提交编写一个名字(eg.first commit)后点击Commit(提交)
   ***注:如果此处报错那就用户名和邮箱没有设置好***
5.提交之后代码在本地仓库就保存好了，如果对代码再次修改，保存之后，对第二次修改起个名字就行，此时甚至能看到第一次和第二次不一样的地方在哪里
## Git远程提交
1. 保存到本地仓库后，还是原来那个地方，点击Publish Branch，(注：若第一次发布到Github，需要保证默认浏览器已经登录Github账号，点击Continue，授予Vscode权限，最终点击Authorize Visual-Studio-Code)
2. 此时VsCode上边框多两个选项，private为私有，public为公开，即你选择是否将代码公开
3. 如果上传失败，在搜索引擎上面搜索git set proxy设置代理
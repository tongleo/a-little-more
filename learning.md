###   css3圆形按钮
[w3cPlus链接](http://www.w3cplus.com/demo/495.html)
###   mobiscroll
2016-11-21  mobiscroll在dateFormat为"yyyy-mm-dd"情况下会出现初始化后点击的第一次不管文本框的内容是什么年份都是一个固定的年份（我在项目中遇到的是2000年，猜测和起始年份有关），格式改为“yy-mm-dd”就可以了
###   react教程 
[github地址](https://github.com/theJian/build-a-hn-front-page)
[一个人员管理（react）](http://blog.csdn.net/a153375250/article/details/52667739)

###  sass教程
[sass教程](https://speakerdeck.com/w3cplus/sassdai-lai-de-bian-ge),wscPlus大漠

### git 关联远程仓库[原链接](http://www.jianshu.com/p/dcbb8baa6e36)

### git 从远程仓库更新代码到本地仓库

#### 1. git remote -v 
```git操作
1. eoecn   https://github.com/eoecn/android-app.git (fetch)
2. eoecn   https://github.com/eoecn/android-app.git  (push)
3. origin  https://github.com/com360/android-app.git  (fetch)
4. origin  https://github.com/com360/android-app.git (push)
5. su@SUCHANGLI /e/eoe_client/android-app (master)
```
从上面的结果可以看出，远程仓库有两个，一个是一个是eoecn，一个是origin

#### 2.从远程获取最新版本到本地
```git操作
1. $ git fetch origin master:temp
2. From https://github.com/com360/android-app
3.  * [new branch]      master     -> temp
4. su@SUCHANGLI /e/eoe_client/android-app (master)
```
git fetch origin master:temp 这句命令的意思是：从远程的origin仓库的master分支下载到本地并新建一个分支temp
#### 3.比较本地的仓库和远程参考的区别
```git操作
1. $ git diff temp 
2. su@SUCHANGLI /e/eoe_client/android-app (master)
```
命令的意思是：比较master分支和temp分支的不同
由于我的没有区别就没有显示其他信息
#### 4合并temp分支到master分支
```git操作
1. $ git merge temp
2. Already up-to-date.
3. su@SUCHANGLI /e/eoe_client/android-app (master)
```
由于没有区别，所以显示Already up-to-date.

合并的时候可能会出现冲突
#### 5.如果不想要temp分支了，可以删除此分支
```git操作
1. $ git branch -d temp
2. Deleted branch temp (was d6d48cc).
3. su@SUCHANGLI /e/eoe_client/android-app (master)
```
如果该分支没有合并到主分支会报错，可以用以下命令强制删除git branch -D <分支名>
原文链接:[点击打开链接](http://www.eoeandroid.com/portal.php)

###git vim操作

但是git bush使用vi命令创建文件时进入到vim编辑器后，我不知道怎么退出，查了下发现一个方法：

 

方法：一直按住esc ，再连续按大写的z两次就退出来了。

但实际上，我发现，只要你按住shift键盘，下面的这些命令都可以用：
```
1 如果你想编辑某个文档 可以直接编辑的如你有文档AA 可以用vi AA 【注意：必须在AA所在的目录下】
2 如果没有文档而且你又想编辑就可以直接编辑vi aa【名字你可以随便命名】
3 也可以先建立一个文档touch aa 然后再编辑vi aa
4 编辑器有三种模式 1 命令行模式 2 末行模式 3 输入模式
5 按Esc 就可以进入命令行模式也是系统默认模式
6 输入模式可以按 o i a 都可以进入 退出可以进入末行和命令行模式
7 末行模式可以按ctrl+；它的主要功能是退出编辑器 也可以保存退出文档
8 q! 【强制退出不保存】 q【退出不保存】 wq【退出并保存后面也可以加个！】
9 在输入模式和命令行模式命令很多 如果你想具体知道哪些你可以在和我说
10 如复制（yy）粘贴（p) 删除（d）等等
```
只是，用wq的时候，要先esc，然后按住shift键，出现下面这个界面时才可以输入命令：[原文链接](http://www.cnblogs.com/macliu/p/6062917.html)

[git详细教程](http://www.yiibai.com/git/git_update_operation.html)


### webpack 教程
[链接](http://www.w2bc.com/Article/50764)
### npm命令介绍
npm介绍
3.1、说明：npm（node package manager）nodejs的包管理器，用于node插件管理（包括安装、卸载、管理依赖等）；
3.2、使用npm安装插件：命令提示符执行npm install <name> [-g] [--save-dev]；
3.2.1、<name>：node插件名称。例：npm install gulp-less --save-dev
3.2.2、-g：全局安装。将会安装在C:\Users\Administrator\AppData\Roaming\npm，并且写入系统环境变量；  非全局安装：将会安装在当前定位目录；  全局安装可以通过命令行在任何地方调用它，本地安装将安装在定位目录的node_modules文件夹下，通过require()调用；
3.2.3、--save：将保存配置信息至package.json（package.json是nodejs项目配置文件）；
3.2.4、-dev：保存至package.json的devDependencies节点，不指定-dev将保存至dependencies节点；一般保存在dependencies的像这些express/ejs/body-parser等等。
3.2.5、为什么要保存至package.json？因为node插件包相对来说非常庞大，所以不加入版本管理，将配置信息写入package.json并将其加入版本管理，其他开发者对应下载即可（命令提示符执行npm install，则会根据package.json下载所有需要的包，npm install --production只下载dependencies节点的包）。
3.3、使用npm卸载插件：npm uninstall <name> [-g] [--save-dev]  PS：不要直接删除本地插件包
3.3.1、删除全部插件：npm uninstall gulp-less gulp-uglify gulp-concat ……???太麻烦
3.3.2、借助rimraf：npm install rimraf -g 用法：rimraf node_modules
3.4、使用npm更新插件：npm update <name> [-g] [--save-dev]
3.4.1、更新全部插件：npm update [--save-dev]
3.5、查看npm帮助：npm help
3.6、当前目录已安装插件：npm list
PS：npm安装插件过程：从http://registry.npmjs.org下载对应的插件包（该网站服务器位于国外，所以经常下载缓慢或出现异常），解决办法往下看cnpm。

### Browsersync
[Browsersync](http://www.browsersync.cn/)
[Browsersync + Gulp.js - Browsersync中文网](http://www.browsersync.cn/docs/gulp/)



[谷歌跨域插件](https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi)
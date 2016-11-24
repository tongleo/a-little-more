###   css3圆形按钮
[w3cPlus链接](http://www.w3cplus.com/demo/495.html)
###   mobiscroll
2016-11-21  mobiscroll在dateFormat为"yyyy-mm-dd"情况下会出现初始化后点击的第一次不管文本框的内容是什么年份都是一个固定的年份（我在项目中遇到的是2000年，猜测和起始年份有关），格式改为“yy-mm-dd”就可以了
###   react教程 
[github地址](https://github.com/theJian/build-a-hn-front-page)
[一个人员管理（react）](http://blog.csdn.net/a153375250/article/details/52667739)

###  sass教程
[sass教程](https://speakerdeck.com/w3cplus/sassdai-lai-de-bian-ge),wscPlus大漠

### git 从远程仓库更新代码到本地仓库
```git操作
#### 1. git remote -v 
2. eoecn   https://github.com/eoecn/android-app.git (fetch)
3. eoecn   https://github.com/eoecn/android-app.git  (push)
4. origin  https://github.com/com360/android-app.git  (fetch)
5. origin  https://github.com/com360/android-app.git (push)
6. su@SUCHANGLI /e/eoe_client/android-app (master)
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

###   css3Բ�ΰ�ť
[w3cPlus����](http://www.w3cplus.com/demo/495.html)
###   mobiscroll
2016-11-21  mobiscroll��dateFormatΪ"yyyy-mm-dd"����»���ֳ�ʼ�������ĵ�һ�β����ı����������ʲô��ݶ���һ���̶�����ݣ�������Ŀ����������2000�꣬�²����ʼ����йأ�����ʽ��Ϊ��yy-mm-dd���Ϳ�����
###   react�̳� 
[github��ַ](https://github.com/theJian/build-a-hn-front-page)
[һ����Ա����react��](http://blog.csdn.net/a153375250/article/details/52667739)

###  sass�̳�
[sass�̳�](https://speakerdeck.com/w3cplus/sassdai-lai-de-bian-ge),wscPlus��Į

### git ��Զ�ֿ̲���´��뵽���زֿ�
```git����
#### 1. git remote -v 
2. eoecn   https://github.com/eoecn/android-app.git (fetch)
3. eoecn   https://github.com/eoecn/android-app.git  (push)
4. origin  https://github.com/com360/android-app.git  (fetch)
5. origin  https://github.com/com360/android-app.git (push)
6. su@SUCHANGLI /e/eoe_client/android-app (master)
```
������Ľ�����Կ�����Զ�ֿ̲���������һ����һ����eoecn��һ����origin

#### 2.��Զ�̻�ȡ���°汾������
```git����
1. $ git fetch origin master:temp
2. From https://github.com/com360/android-app
3.  * [new branch]      master     -> temp
4. su@SUCHANGLI /e/eoe_client/android-app (master)
```
git fetch origin master:temp ����������˼�ǣ���Զ�̵�origin�ֿ��master��֧���ص����ز��½�һ����֧temp
#### 3.�Ƚϱ��صĲֿ��Զ�̲ο�������
```git����
1. $ git diff temp 
2. su@SUCHANGLI /e/eoe_client/android-app (master)
```
�������˼�ǣ��Ƚ�master��֧��temp��֧�Ĳ�ͬ
�����ҵ�û�������û����ʾ������Ϣ
#### 4�ϲ�temp��֧��master��֧
```git����
1. $ git merge temp
2. Already up-to-date.
3. su@SUCHANGLI /e/eoe_client/android-app (master)
```
����û������������ʾAlready up-to-date.

�ϲ���ʱ����ܻ���ֳ�ͻ
#### 5.�������Ҫtemp��֧�ˣ�����ɾ���˷�֧
```git����
1. $ git branch -d temp
2. Deleted branch temp (was d6d48cc).
3. su@SUCHANGLI /e/eoe_client/android-app (master)
```
����÷�֧û�кϲ�������֧�ᱨ����������������ǿ��ɾ��git branch -D <��֧��>
ԭ������:[���������](http://www.eoeandroid.com/portal.php)

###   css3Բ�ΰ�ť
[w3cPlus����](http://www.w3cplus.com/demo/495.html)
###   mobiscroll
2016-11-21  mobiscroll��dateFormatΪ"yyyy-mm-dd"����»���ֳ�ʼ�������ĵ�һ�β����ı����������ʲô��ݶ���һ���̶�����ݣ�������Ŀ����������2000�꣬�²����ʼ����йأ�����ʽ��Ϊ��yy-mm-dd���Ϳ�����
###   react�̳� 
[github��ַ](https://github.com/theJian/build-a-hn-front-page)
[һ����Ա����react��](http://blog.csdn.net/a153375250/article/details/52667739)

###  sass�̳�
[sass�̳�](https://speakerdeck.com/w3cplus/sassdai-lai-de-bian-ge),wscPlus��Į

### git ����Զ�ֿ̲�[ԭ����](http://www.jianshu.com/p/dcbb8baa6e36)

### git ��Զ�ֿ̲���´��뵽���زֿ�

#### 1. git remote -v 
```git����
1. eoecn   https://github.com/eoecn/android-app.git (fetch)
2. eoecn   https://github.com/eoecn/android-app.git  (push)
3. origin  https://github.com/com360/android-app.git  (fetch)
4. origin  https://github.com/com360/android-app.git (push)
5. su@SUCHANGLI /e/eoe_client/android-app (master)
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

###git vim����

����git bushʹ��vi������ļ�ʱ���뵽vim�༭�����Ҳ�֪����ô�˳��������·���һ��������

 

������һֱ��סesc ������������д��z���ξ��˳����ˡ�

��ʵ���ϣ��ҷ��֣�ֻҪ�㰴סshift���̣��������Щ��������ã�
```
1 �������༭ĳ���ĵ� ����ֱ�ӱ༭���������ĵ�AA ������vi AA ��ע�⣺������AA���ڵ�Ŀ¼�¡�
2 ���û���ĵ�����������༭�Ϳ���ֱ�ӱ༭vi aa��������������������
3 Ҳ�����Ƚ���һ���ĵ�touch aa Ȼ���ٱ༭vi aa
4 �༭��������ģʽ 1 ������ģʽ 2 ĩ��ģʽ 3 ����ģʽ
5 ��Esc �Ϳ��Խ���������ģʽҲ��ϵͳĬ��ģʽ
6 ����ģʽ���԰� o i a �����Խ��� �˳����Խ���ĩ�к�������ģʽ
7 ĩ��ģʽ���԰�ctrl+��������Ҫ�������˳��༭�� Ҳ���Ա����˳��ĵ�
8 q! ��ǿ���˳������桿 q���˳������桿 wq���˳����������Ҳ���ԼӸ�����
9 ������ģʽ��������ģʽ����ܶ� ����������֪����Щ������ں���˵
10 �縴�ƣ�yy��ճ����p) ɾ����d���ȵ�
```
ֻ�ǣ���wq��ʱ��Ҫ��esc��Ȼ��סshift�������������������ʱ�ſ����������[ԭ������](http://www.cnblogs.com/macliu/p/6062917.html)

[git��ϸ�̳�](http://www.yiibai.com/git/git_update_operation.html)


### webpack �̳�
[����](http://www.w2bc.com/Article/50764)
### npm�������
npm����
3.1��˵����npm��node package manager��nodejs�İ�������������node�������������װ��ж�ء����������ȣ���
3.2��ʹ��npm��װ�����������ʾ��ִ��npm install <name> [-g] [--save-dev]��
3.2.1��<name>��node������ơ�����npm install gulp-less --save-dev
3.2.2��-g��ȫ�ְ�װ�����ᰲװ��C:\Users\Administrator\AppData\Roaming\npm������д��ϵͳ����������  ��ȫ�ְ�װ�����ᰲװ�ڵ�ǰ��λĿ¼��  ȫ�ְ�װ����ͨ�����������κεط������������ذ�װ����װ�ڶ�λĿ¼��node_modules�ļ����£�ͨ��require()���ã�
3.2.3��--save��������������Ϣ��package.json��package.json��nodejs��Ŀ�����ļ�����
3.2.4��-dev��������package.json��devDependencies�ڵ㣬��ָ��-dev��������dependencies�ڵ㣻һ�㱣����dependencies������Щexpress/ejs/body-parser�ȵȡ�
3.2.5��ΪʲôҪ������package.json����Ϊnode����������˵�ǳ��Ӵ����Բ�����汾������������Ϣд��package.json���������汾�������������߶�Ӧ���ؼ��ɣ�������ʾ��ִ��npm install��������package.json����������Ҫ�İ���npm install --productionֻ����dependencies�ڵ�İ�����
3.3��ʹ��npmж�ز����npm uninstall <name> [-g] [--save-dev]  PS����Ҫֱ��ɾ�����ز����
3.3.1��ɾ��ȫ�������npm uninstall gulp-less gulp-uglify gulp-concat ����???̫�鷳
3.3.2������rimraf��npm install rimraf -g �÷���rimraf node_modules
3.4��ʹ��npm���²����npm update <name> [-g] [--save-dev]
3.4.1������ȫ�������npm update [--save-dev]
3.5���鿴npm������npm help
3.6����ǰĿ¼�Ѱ�װ�����npm list
PS��npm��װ������̣���http://registry.npmjs.org���ض�Ӧ�Ĳ����������վ������λ�ڹ��⣬���Ծ������ػ���������쳣��������취���¿�cnpm��

### Browsersync
[Browsersync](http://www.browsersync.cn/)
[Browsersync + Gulp.js - Browsersync������](http://www.browsersync.cn/docs/gulp/)



[�ȸ������](https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi)
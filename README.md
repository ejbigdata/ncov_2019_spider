ncov_2019_spider
-
2019 ��״�����������档�������ݿ��ӻ���

## ��Ŀ����
�������ݷ���

## ������Դ
����ҽ������1.24�ſ�ʼ�ɼ���⣬���Թ��̰�����24�ź�����ݡ�

## ����չʾ
1. ![](http://baidu.com/pic/doge.png )
2. ![](http://baidu.com/pic/doge.png )
3. ![](http://baidu.com/pic/doge.png )
4. ![](http://baidu.com/pic/doge.png )





##����ջ
1. mongodb ���ڴ洢�ɼ�����
2. mysql 5.7 ���ڴ洢��mogodb�ɼ�������
3. python 3.7 �ɼ����ݺ�ת��mongodb���ݵ�mysql

## FAQ
1. ΪʲôҪ��2�����ݿ�
һ�����û���֪��ʹ��nosql�����������Լ�����һЩ��ѯ��ʱ����sql����˳�֡�

2. ���ᰲװ�Ͳ�����ֻ��Ҫ����
��ISSUE,����ϵ΢�ţ�ajun-guo


##��װ�Ͳ���
 
#### mongodb ���ڲɼ������ݿ����
��װ����for mac :https://www.runoob.com/mongodb/mongodb-osx-install.html
����mongo ������
mongod --dbpath d:/workspace/mongodb
export PATH=/usr/local/mongodb/bin:$PATH && sudo mongod

#### mysql server��װ

##### ж��mysql(�Ǳ�Ҫ����)
```bash
sudo rm /usr/local/mysql
sudo rm -rf /usr/local/mysql*
sudo rm -rf /Library/StartupItems/MySQLCOM
sudo rm -rf /Library/PreferencePanes/My*
rm -rf ~/Library/PreferencePanes/My*
sudo rm -rf /Library/Receipts/mysql*
sudo rm -rf /Library/Receipts/MySQL*
sudo rm -rf /var/db/receipts/com.mysql.*
networksetup -setairportpower en0 off && networksetup -setairportpower en0 on

���� �� http://dev.mysql.com/get/Downloads/MySQL-5.7/mysql-5.7.10-osx10.9-x86_64.dmg
��װ������https://www.cnblogs.com/kimbo/p/8724595.html
root@localhost: 4O=ucCLx9y%3
/usr/local/mysql-5.7.10-osx10.9-x86_64/bin
```



##### ����mysql����(�Ǳ�Ҫ����)
```
1. �ر�mysql����
sudo /usr/local/mysql/support-files/mysql.server stop ����ϵͳƫ�����и� MySQL ��ر�
2.����mysqlĿ¼��
/usr/local/mysql-5.7.10-osx10.9-x86_64/bin
3.�õ�Ȩ��
sudo su
4.����mysql����
./mysqld_safe --skip-grant-tables &? ������ϵͳ����п���
5.�ؿ��ն�
mysql -uroot -p ����ʾ��������ʱ������뼴��
6. �õ�Ȩ�ޣ������޸����룩
flush privileges;
7.�޸�����
set password for 'root'@'localhost'=password('root');
set password for 'root'@'localhost'=password('root');
```
 
#### ��װnavicat for mysql
���ص�ַ��http://www.pc6.com/mac/111878.html
���նˣ����룺sudo spctl --master-disable �س�����ƫ�����õİ�ȫ������˽�������κ���Դ�����´�Navicat for MySQL��OK��



#### ��װpython������
python3 -m pip install -r requirements.txt



### ����˵��
crawler.py ����������������ļ�
python crawler.py 
�����󣬾ͻ�ѭ���������ȡ����������⵽mongo

spider.py ��mongo 2 mysql ������ת����
��Ҫ�Ƿ������ʹ��sql �����ݲ�ѯ���о���
Ҳ��Ҫ����������ʵʱת�����ݵ�mysql
python spider.py

���ݿ����ƣ�ncov
��ѯʵ������ҵ��.sql

�� ��
dxyarea  ʡ������
dxyarea_city ���м�����
dxyoverall �������ݸ���


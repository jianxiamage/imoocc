部署手册:
1.执行命令，安装模块
　　pip install -r ./requirements.txt

2.imoocc-master/admin/settings/settings.py
  确认数据库信息，包括数据库名称，用户名，密码等

3.登录mysql,创建数据库，创建用户，设置密码。

　　　　　　　　create database imoocc;

　　　　　　　　grant all on imoocc.* to imoocc@"localhost" identified by 'imoocccom';

4.生成数据
　　　　　　　　python ./manage.py makemigrations

　　　　　　　　python ./manage.py migrate

5.运行工程

　　　　　　　　python ./manage.py runserver 0.0.0.0:8000


--参考网址：https://www.cnblogs.com/yangjianbo/articles/9798193.html

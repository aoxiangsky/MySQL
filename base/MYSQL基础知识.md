# MYSQL 基础知识

## 数据库的基本概念

    1. 数据库的英文单词：DataBase	简称：DB
    2. 什么是数据库？
    	* 用于存储和管理数据的仓库
    3. 数据库的特点
    	1. 持久化存储数据。其实数据库就是一个文件系统
    	2. 方便存储和管理数据
    	3. 使用了统一的方式操作数据库
    4. 常见的数据库软件
    Oracle
    MySQL
    Microsoft SQL Server
    MongoDB
    等等。。。

- MySQL 服务启动

1. 命令行输入 services.msc 查看 windows 服务列表
2. 命令行输入 net start(stop) mysql 启动，停止 mysql 服务

- MySql 登录

1. mysql -u root -p
2. 输入密码

3. mysql -h（ip 地址） -uroot -p(连接密码)

4. mysql --host=127.0.0.1 --user=root --password=root

- 退出

1. 命令行输入 exit 或 quit

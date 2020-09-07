# SQL

1. 什么是 SQL

   Structured Query Language: 结构化查询语言
   其实就是定义了操作所有关系型数据库的规则
   每一种数据库操作的方式存在不一样的地方，称为“方言”

2. SQL 通用语法

   1. SQL 语句可以单行或多行书写，以分号结尾。
   2. 可使用空格和缩进增强语句的可读性
   3. MySql 数据库的 SQL 语句不区分大小写，关键字建议使用大写
   4. 3 种注释
      _ 单行注释: -- 注释内容 或 # 注释内容(mysql 特有)
      _ 多行注释: /_ 注释 _/

3. SQL 分类
   1. DDL(Data Definition Language)数据定义语言
      用来定义数据库对象：数据库，表，列等。关键字：create, drop,alter 等
   2. DML(Data Manipulation Language)数据操作语言
      用来对数据库中表的数据进行增删改。关键字：insert, delete, update 等
   3. DQL(Data Query Language)数据查询语言
      用来查询数据库中表的记录(数据)。关键字：select, where 等
   4. DCL(Data Control Language)数据控制语言(了解)
      用来定义数据库的访问权限和安全级别，及创建用户。关键字：GRANT， REVOKE 等

## DDL：操作数据库，表

### 操作数据库：CRUD

    1. C(Create):创建
    	* 创建数据库：
    		* create database 数据库名称;
    	* 创建数据库，判断不存在，再创建：
    		* create database if not exists 数据库名称;
    	* 创建数据库，并指定字符集
    		* create database 数据库名称 character set 字符集名;

    	* 练习： 创建db4数据库，判断是否存在，并制定字符集为gbk
    		* create database if not exists db4 character set gbk;
    2. R(Retrieve)：查询
    	* 查询所有数据库的名称:
    		* show databases;
    	* 查询某个数据库的字符集:查询某个数据库的创建语句
    		* show create database 数据库名称;
    3. U(Update):修改
    	* 修改数据库的字符集
    		* alter database 数据库名称 character set 字符集名称;
    4. D(Delete):删除
    	* 删除数据库
    		* drop database 数据库名称;
    	* 判断数据库存在，存在再删除
    		* drop database if exists 数据库名称;
    5. 使用数据库
    	* 查询当前正在使用的数据库名称
    		* select database();
    	* 使用数据库
    		* use 数据库名称;

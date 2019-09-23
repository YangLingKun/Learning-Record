#### mysql常用操作

##### 3306端口被占用

- netstat -ano
- netstat -ano|findstr "3306"
- taskkill /pid 数字 /f

##### 自增id乱序重排

alter table 表名 drop column id;

alter table 表名 add id mediumint(8) not null primary key auto_increment first;

##### 添加索引

ALTER TABLE  表名  ADD INDEX 索引名 （列名 ) 

##### 删除字段

 ALTER TABLE 表名 DROP 列名;

##### 修改字段类型

alter table 表名 modify column 列名 类型;

##### 添加字段

ALTER TABLE 表名 ADD COLUMN 列名 VARCHAR(100) DEFAULT NULL COMMENT '姓名'

##### 修改字段的注释

alter table 表名 modify column 列名 int default 0 not null comment '修改后的字段注释';

##### 修改字段

alter table <表名> change <字段名> <字段新名称> <字段的类型>。
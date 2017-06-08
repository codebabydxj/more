# More

## wamp

* w   windows
* a    apache
* m   mysql
* p    php

* ## 协议
* file://    本地协议

* http://   网络协议

* https://    网络协议（更安全）

* ftp://    文件传输协议（上传到服务）

* svn://   文件传输协议

## 控制台操作数据库

* net start mysql  // 开启数据库服务
* net stop mysql  // 关闭数据库服务

* mysql -hlocalhost -uroot -p   // 进入本地数据库

* show databases // 显示本地数据库

* exit;  // 退出mysql

* show tables  // 显示所有数据库

* use class  // 打开指定数据库

* desc stu  // 查看表结构

* create database class  //  创建数据库

* create table stu...  // 创建表

* drop database class  // 删除数据库

* drop table stu  // 删除表

## AMD&CMD

> 模块化编程的方法

#### AMD

> 依赖前置，提前执行，2.0之后可以依赖就近

##### require.js

```
define(["a","b"],function(a,b){//函数体})
```

#### CMD

> 依赖就近，延迟执行

##### sea.js

```
define(function(require,exports,module){
    var a=require("./a");
    //函数体
})
```



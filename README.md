# Mysql（# Python（基于v3.5.2）


###  一、小例子<br>
----------------------

###  二、Tips<br>
----------------------
####    1、概念理解
####      1、字符集：
          Mysql的字符集，如果使用的话，就用utf8m-b4,它的utf8是专属的编码，只支持每个字符最多三个字节，而真正的UTF-8是四个（最明显
    的问题是utf8不支持emoji和很多繁体字）。
          
####      2、修改密码：新版本Mysql的mysql-user表里面，是没有password字段的，所以修改密码要这样：
          update user set authentication_string=password('123') where user='root';

### 参考
-----------

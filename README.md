crud
====

CRUD is Really Urgly coDed -- 课设毕设快速原型

表设计原则

1、每个表必须有id，自增类型

2、每个表id后的第一个字符型字段被当做外键关联的显示值

3、外键一律以表名_id进行命名。

datadic表用于翻译英文表名列名到中文,建表语句在db.sql。

默认账号admin 密码admin， 除config/datadic/privilege/user四张系统表以外，样例表可以删除。

符合上述原则设计表，自动实现菜单、各表增删改，用于快速建立小型系统原型。

支持超文本编辑、文件上传。

新增权限管理，guest用户，显示内容单页含二维码。

数据库配置文件在WEB-INF/db.prop

![image](https://github.com/zhblue/crud/blob/master/crud/crud.png)

正常连接数据库后，新建符合上述要求的数据表，刷新页面会自动出现新的菜单，点击可以展开数据进行增删改。

需要中文含义，在数据字典表中进行添加即可，刷新页面立刻生效。




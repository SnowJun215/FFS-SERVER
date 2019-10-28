# 启动错误
## redis连接失败
> ReplyError: Ready check failed: NOAUTH Authentication required.

解决办法
> redis设置了连接密码，需要配置密码参数，参数名为password

## 数据库连接失败
>SequelizeConnectionError: Client does not support authentication protocol requested by server; consi

解决办法
> ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password'
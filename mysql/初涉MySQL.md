## MySQL登录
参数详解：  
-D, --database=name --->打开指定数据库  
--delimite=name     --->指定分隔符  
-h, host=name       --->服务器名称  
--prompt=name       --->设置提示符  
-V, --version       --->输出版本信息并且推出  
```bash
# -u是user的简写；-p是password；-P是port的简写
mysql -uroot -p -P
```
## 修改MySQL提示符
```bash
# 登录时修改
mysql -uroot -p123456 --prompt yesixuan>
# 登录后修改
prompt /h
```
除了输入具名提示符，还可以输入代名符：
\D，当前完整日期  
\d，当前数据库  
\h，服务器名称  
\u，当前用户  

## 常用命令
- 创建数据库
```bash
CREATE {DATABASE | SCHEMA} [IF NOT EXISTS] db_name [DEFAULT] CHARACTER [=] charset_name  
```
- 修改数据库编码格式
```bash
# 查看某数据库的编码格式
SHOW CREATE DATABASE db_name
# 修改已创建的数据库编码格式
ALTER {DATABASE | SCHEMA}  db_name [DEFAULT] CHARACTER [=] charset_name
```
- 删除数据库
```bash
DROP {DATABASE | SCHEMA} [IF NOT EXISTS] db_name
```

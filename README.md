# MySQL_install
MySQL安装过程（zip格式文件）  
1、下载zip格式的安装软件

2、解压到本地

3、在解压后的文件夹中新建mysql.ini文件，内容见[mysql.ini](mysql.ini)

4、把解压后的bin路径配置到环境变量

5、以管理员的身份打开命令提示符

6、配置文件，输入命令：mysqld --defaults-file=D:\Program\mysql-5.7.27-winx64\mysql.ini

7、初始化数据库，输入命令：mysqld --initialize-insecure

8、安装数据库，输入命令：mysqld install

9、启动数据库服务，输入命令：net start mysql

10、连接数据库，输入命令：mysql -u root -p

11、设置密码，输入命令：set password = password("root")

注意：此种安装方式不带图形化界面，须自行下载安装，如官方自带的MySQL workbench

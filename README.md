# MySQL_install
MySQL安装过程（zip格式文件）
1、下载zip格式的安装软件

2、解压到本地

3、在解压后的文件夹中新建mysql.ini文件，内容如下
  [mysql]
  # 设置mysql客户端默认字符集
  default-character-set=utf8 
  [mysqld]
  #设置3306端口
  port = 3306 
  # 设置mysql的安装目录
  basedir=D:\Program\mysql-5.7.27-winx64
  # 设置mysql数据库的数据的存放目录
  datadir=D:\Program\mysql-5.7.27-winx64\data
  # 允许最大连接数
  max_connections=200
  # 服务端使用的字符集默认为8比特编码的latin1字符集
  character-set-server=utf8
  # 创建新表时将使用的默认存储引擎
  default-storage-engine=INNODB

4、把解压后的bin路径配置到环境变量

5、以管理员的身份打开命令提示符

6、配置文件，输入命令：mysqld --defaults-file=D:\Program\mysql-5.7.27-winx64\mysql.ini

7、初始化数据库，输入命令：mysqld --initialize-insecure

8、安装数据库，输入命令：mysqld install

9、启动数据库服务，输入命令：net start mysql

10、连接数据库，输入命令：mysql -u root -p

11、设置密码，输入命令：set password = password("root")

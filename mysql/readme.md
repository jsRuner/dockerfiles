#指定数据存储位置
docker run --name mysql -p 3306:3306 -v /Users/ft521/Documents/study/项目/docker/data/mysql:/var/lib/mysql  -e MYSQL_ROOT_PASSWORD=123456 -d mysql:5.7.18

第二个容器。测试是否能获取第一个容器的数据
docker run --name mysql-2 -p 3306:3306 -v /Users/ft521/Documents/study/项目/docker/data/mysql:/var/lib/mysql  -e MYSQL_ROOT_PASSWORD=123456 -d mysql:5.7.18

测试是通过的。


阿里云docker上mysql配置
docker run --name mysql -p 3306:3306 -v /www/mysqldata:/var/lib/mysql  -e MYSQL_ROOT_PASSWORD=Czr7R*^SvaKnnf&% -d registry.cn-hangzhou.aliyuncs.com/qinyujia-test/mysql:latest



docker run --name mysql-master -p 3307:3306 -v /Users/ft521/Documents/study/项目/docker/data/mysql2:/var/lib/mysql  -e MYSQL_ROOT_PASSWORD=123456 -d mysql:latest

docker run --name mysql-slave1 -p 3308:3306 -v /Users/ft521/Documents/study/项目/docker/data/mysql3:/var/lib/mysql  -e MYSQL_ROOT_PASSWORD=123456 -d mysql:latest


change master to master_host='172.17.0.5',master_user='slave_account',master_password='123456',master_log_file='mysql-bin.000001',master_log_pos=598;
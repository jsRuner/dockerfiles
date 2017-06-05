安装镜像
docker pull rabbitmq:management

启动容器

docker run -d --name rabbitmq --publish 5671:5671 \
 --publish 5672:5672 --publish 4369:4369 --publish 25672:25672 --publish 15671:15671 --publish 15672:15672 \
rabbitmq:management

访问管理界面

http://127.0.0.1:15672
账号 guest
密码 guest

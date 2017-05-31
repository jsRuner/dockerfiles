docker run --name php-fpm-4.0 --link=mysql --link=yxy-redis -p 80:80 -it -v /Users/ft521/Documents/study/项目/docker/www:/www -d hiphp-php-fpm:4.0


2017-05-25 09:12:15 更新
增加php的配置项。xdebug的远程调试。
docker build --tag hiphp-php-fpm:4.0 --no-cache  .


2017-05-28 08:11:11

增加php7的构建。

创建php7的容器

docker run --name php-fpm-7 --link=mysql --link=yxy-redis -p 80:80 -it -v /Users/ft521/Documents/study/项目/docker/www:/www -d hiphp-php-fpm-7:1.0


2017-05-31 12:39:53

增加composer的安装。
更新容器的时间

复制项目的配置到外部。
docker cp 

重新构建php56 去掉了对php配置的修改。
docker run --name php-fpm-56-1 --link=mysql --link=yxy-redis -p 80:80 -it -v /Users/ft521/Documents/study/项目/docker/www:/www -d hiphp-php-fpm-56:1.0


2017-05-31 13:54:35
修正date日期
修正php.ini的错误显示问题。
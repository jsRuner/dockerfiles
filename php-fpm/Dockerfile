#基础镜像
FROM centos:7
#作者信息
MAINTAINER 吴文付 <hi_php@163.com>

RUN echo "Asia/shanghai" > /etc/timezone


#更新源. 安装php7
USER root


RUN yum  install -y epel-release
RUN yum install -y http://rpms.famillecollet.com/enterprise/remi-release-7.rpm

#安装nginx
RUN yum install -y nginx


RUN yum install -y wget



RUN yum install -y php70 php70-fpm php70-opcache php70-devel php70-mbstring \
php70-mcrypt php70-mysqlnd php70-pdo php70-mysqli php70-php70unit-PHPUnit php70-pecl-xdebug php70-pecl-xhprof php70-gd php70-redis php70-memcache




#配置文件



#开发端口 
EXPOSE 80 9000



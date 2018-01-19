FROM daocloud.io/library/nginx:1.13.0-alpine

MAINTAINER hi_php@163.com


ADD web/ /usr/share/nginx/html

ADD default.conf /etc/nginx/conf.d

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]


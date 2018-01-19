FROM daocloud.io/library/php:7.0.20-fpm
RUN sed -i -e 's/listen = 127.0.0.1:9000/listen = 9000/' /usr/local/etc/php-fpm.d/www.conf
#启动php
CMD ["php-fpm"]

#nginx 重起
docker exec -it dnmp-nginx nginx -s reload

#php 交互
docker exec -it dnmp-php /bin/bash

#php 权限
chown -R www-data:www-data /var/www/html

#更新容器
docker-compose up --force-recreate

https://www.awaimai.com/2120.html

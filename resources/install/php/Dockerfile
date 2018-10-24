FROM centos:latest

#tools
RUN yum -y install epel-release
RUN rpm -Uvh http://rpms.famillecollet.com/enterprise/remi-release-7.rpm
RUN yum -y install git wget jwhois bind-utils screen

# php
RUN yum --enablerepo=remi-php72 -y install php-fpm php-common
RUN yum --enablerepo=remi-php72 -y install php-opcache php-pecl-apcu php-cli php-pear php-pdo php-mysqlnd php-pgsql php-pecl-mongodb php-pecl-redis php-pecl-memcache php-pecl-memcached php-pecl-swoole4 php-pecl-seaslog php-pecl-libsodium2 php-pecl-nsq3 php-gd php-mbstring php-mcrypt php-xml php-devel


# Composer
#RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin/ --filename=composer
#RUN chmod +x /usr/bin/composer
#RUN composer config -g --unset repos.packagist

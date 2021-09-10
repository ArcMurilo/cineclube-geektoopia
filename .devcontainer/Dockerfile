FROM php:7-alpine

RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
    php composer-setup.php --install-dir=/usr/local/bin --filename=composer && \
    rm composer-setup.php

RUN docker-php-ext-install pdo pdo_mysql && \
    docker-php-ext-enable pdo pdo_mysql

RUN apk add --update nodejs npm

RUN composer global require squizlabs/php_codesniffer
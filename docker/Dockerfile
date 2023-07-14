FROM php:8.0.2-fpm

RUN apt-get update && apt-get install -y \
    git \
    curl \
    zip \
    unzip

COPY ./php/webdev.ini /usr/local/etc/php/conf.d
COPY ./php/webdev.pool.conf /usr/local/etc/php-fpm.d/

WORKDIR /var/www
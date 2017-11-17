FROM php:7.1-fpm

RUN docker-php-ext-install -j$(nproc) pdo_mysql


WORKDIR /app

RUN usermod -u 1000 www-data

FROM php:7.1-alpine

RUN docker-php-ext-install -j$(nproc) pdo_mysql


WORKDIR /app


WORKDIR /app

RUN usermod -u 1000 www-data

CMD php artisan horizon
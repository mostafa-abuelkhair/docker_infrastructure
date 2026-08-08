FROM php:8.3-fpm

RUN docker-php-ext-install pdo pdo_mysql pdo_pgsql opcache \
    && pecl install redis \
    && docker-php-ext-enable redis

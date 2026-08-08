FROM php:8.3-fpm-alpine

RUN docker-php-ext-install pdo pdo_mysql pdo_pgsql opcache \
    && apk add --no-cache $PHPIZE_DEPS \
    && pecl install redis \
    && docker-php-ext-enable redis \
    && apk del $PHPIZE_DEPS

FROM php:8-apache

RUN apt-get update && apt-get install -y git zip\
    && docker-php-ext-install pdo_mysql

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
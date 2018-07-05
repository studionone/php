FROM php:apache

RUN apt-get update && apt-get install -y wget libpq-dev \
    && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install pdo pdo_pgsql pgsql

RUN a2enmod rewrite

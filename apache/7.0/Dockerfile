FROM php:7.0-apache

COPY ../config/php-config.sh /opt/

RUN apt-get update && apt-get install -y wget libpq-dev \
    && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install pdo pdo_pgsql pgsql \
    && sh /opt/php-config.sh \
    && a2enmod rewrite

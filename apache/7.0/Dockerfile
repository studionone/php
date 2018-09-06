FROM php:7.0-apache

RUN apt-get update && apt-get install -y wget libpq-dev \
    && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install pdo pdo_pgsql pgsql \
    && echo \
    "file_uploads = On\n" \
    "memory_limit = 500M\n" \
    "upload_max_filesize = 500M\n" \
    "post_max_size = 500M\n" \
    "max_execution_time = 600\n" \
    > /usr/local/etc/php/conf.d/uploads.ini \
    && a2enmod rewrite

FROM php:apache

ENV FPM_HOST fpm
ENV FPM_PORT 9000
ENV VHOST_FOLDER /var/www/html/

RUN a2enmod rewrite proxy proxy_fcgi

COPY ./../config/using-fpm.conf /etc/apache2/sites-available/000-default.conf

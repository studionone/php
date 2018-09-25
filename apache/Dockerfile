FROM php:7.0-apache

COPY ./config/apache-config.sh /opt/

RUN sh /opt/apache-config.sh && rm /opt/apache-config.sh

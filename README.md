# studionone/php
Clone of official PHP with some improvements.

## Supported tags and respective `Dockerfile` links
- [`apache` (*apache/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/Dockerfile)
- [`7.0-apache` (*apache/7.0/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/7.0/Dockerfile)
- [`7.1-apache` (*apache/7.1/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/7.1/Dockerfile)
- [`7.2-apache` (*apache/7.2/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/7.2/Dockerfile)
- [`apache-fpm` (*apache/fpm/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/fpm/Dockerfile)
- [`7.0-apache-fpm` (*apache/7.0/fpm/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/7.0/fpm/Dockerfile)
- [`7.1-apache-fpm` (*apache/7.1/fpm/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/7.1/fpm/Dockerfile)
- [`7.2-apache-fpm` (*apache/7.2/fpm/Dockerfile*)](https://github.com/studionone/php/blob/master/apache/7.2/fpm/Dockerfile)
- [`nginx-fpm` (*nginx/Dockerfile*)](https://github.com/studionone/php/blob/master/nginx/Dockerfile)

## Standard Apache images
### `apache`, `7.0-apache`, `7.1-apache` and `7.2-apache`
- Apache2 module `mod_rewrite` is enabled
- PHP extensions `pdo`, `pdo_pgsql` and `pgsql`
- PHP directive `file_uploads` set to `On`
- PHP directive `memory_limit` set to `512M`
- PHP directive `upload_max_filesize` set to `512M`
- PHP directive `post_max_size` set to `512M`
- PHP directive `max_execution_time` set to `600`

## FPM-dependant Apache images
### `apache-fpm`, `7.0-apache-fpm`, `7.1-apache-fpm` and `7.2-apache-fpm`
- Apache2 module `rewrite` is enabled
- Apache2 module `proxy` is enabled
- Apache2 module `proxy_fcgi` is enabled
- Environment variable `FPM_HOST` defaults to `fpm`
- Environment variable `FPM_PORT` defaults to `9000`
- Environment variable `VHOST_FOLDER` defaults to `/var/www/html/`

## FPM-dependant Nginx images
### `nginx-fpm`
- The FPM host must be `fpm`
- The FPM host must listen on `9000`
- The codebase goes to `/var/www/html`

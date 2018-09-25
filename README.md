# studionone/php
Clone of official PHP with some improvements.

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
## `apache-fpm`, `7.0-apache-fpm`, `7.1-apache-fpm` and `7.2-apache-fpm`
- Apache2 module `rewrite` is enabled
- Apache2 module `proxy` is enabled
- Apache2 module `proxy_fcgi` is enabled
- Environment variable `FPM_HOST` defaults to `fpm`
- Environment variable `FPM_PORT` defaults to `9000`
- Environment variable `VHOST_FOLDER` defaults to `/var/www/html/`

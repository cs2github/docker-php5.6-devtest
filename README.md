# PHP-FPM 5.6 Docker container

A Docker container with PHP-FPM 5.6 based on php:5.6-fpm-alpine. 


# Important information

**PHP-FPM is running with uid/gid 1008.**


# PHP-FM 5.6 Docker container

> Alpine 3.4

> PHP-FPM 5.6

## Following PHP extensions are available:

> curl 

> gd

> geoip (pecl)

> iconv 

> imagick (pecl)

> imap 

> intl 

> ldap 

> memcache (pecl)

> mcrypt 

> mysqli 

> opcache 

> pdo

> pdo_mysql 

> redis (pecl)

> soap 

> xdebug (pecl)

> xsl 

 
## Usage

You need to define a host directory with php files (usually document root) which will be mounted into the container. 

```
docker run -d \
  -v SOME_HOST_DIRECTORY_WITH_PHP_FILES:/var/www/html \
  --name cs2php56 \
  -p 9000:9000 \
  cs2ag/php5.6-devtest
```
## Exposing ports

The following ports can be exposed in order to use Varnish on container host:

> **9000** `PHP-FPM port`

## Author

* Stefan Preissner (<github@cs2.ch>)  

---

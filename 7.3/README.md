# apache-php

### Run it !
    docker run -p 80:80 --name apache-php  -d pbergen/apache-php:7.3
### Run it with mounted workspace
    docker run -p 80:80 --name apache-php  -d  -v path/to/workspace:/var/www/html pbergen/apache-php:7.3
### PHP 
#### Extensions
- php7.3-common
- php7.3-json
- php7.3-mbstring
- php7.3-apcu
- php7.3-bcmath
- php7.3-cli
- php7.3-curl
- php7.3-fpm
- php7.3-gd
- php7.3-intl
- php7.3-mysql
- php7.3-soap
- php7.3-xml
- php7.3-zip
- php7.3-imagick

#### Configuration
    Configuration File (php.ini) Path: /etc/php/7.3/cli
    Loaded Configuration File:         /etc/php/7.3/cli/php.ini
    Scan for additional .ini files in: /etc/php/7.3/cli/conf.d
    Additional .ini files parsed:      /etc/php/7.3/cli/conf.d/10-mysqlnd.ini,
    /etc/php/7.3/cli/conf.d/10-opcache.ini,
    /etc/php/7.3/cli/conf.d/10-pdo.ini,
    /etc/php/7.3/cli/conf.d/15-xml.ini,
    /etc/php/7.3/cli/conf.d/20-apcu.ini,
    /etc/php/7.3/cli/conf.d/20-bcmath.ini,
    /etc/php/7.3/cli/conf.d/20-calendar.ini,
    /etc/php/7.3/cli/conf.d/20-ctype.ini,
    /etc/php/7.3/cli/conf.d/20-curl.ini,
    /etc/php/7.3/cli/conf.d/20-dom.ini,
    /etc/php/7.3/cli/conf.d/20-exif.ini,
    /etc/php/7.3/cli/conf.d/20-fileinfo.ini,
    /etc/php/7.3/cli/conf.d/20-ftp.ini,
    /etc/php/7.3/cli/conf.d/20-gd.ini,
    /etc/php/7.3/cli/conf.d/20-gettext.ini,
    /etc/php/7.3/cli/conf.d/20-iconv.ini,
    /etc/php/7.3/cli/conf.d/20-imagick.ini,
    /etc/php/7.3/cli/conf.d/20-intl.ini,
    /etc/php/7.3/cli/conf.d/20-json.ini,
    /etc/php/7.3/cli/conf.d/20-mbstring.ini,
    /etc/php/7.3/cli/conf.d/20-mysqli.ini,
    /etc/php/7.3/cli/conf.d/20-pdo_mysql.ini,
    /etc/php/7.3/cli/conf.d/20-phar.ini,
    /etc/php/7.3/cli/conf.d/20-posix.ini,
    /etc/php/7.3/cli/conf.d/20-readline.ini,
    /etc/php/7.3/cli/conf.d/20-shmop.ini,
    /etc/php/7.3/cli/conf.d/20-simplexml.ini,
    /etc/php/7.3/cli/conf.d/20-soap.ini,
    /etc/php/7.3/cli/conf.d/20-sockets.ini,
    /etc/php/7.3/cli/conf.d/20-sysvmsg.ini,
    /etc/php/7.3/cli/conf.d/20-sysvsem.ini,
    /etc/php/7.3/cli/conf.d/20-sysvshm.ini,
    /etc/php/7.3/cli/conf.d/20-tokenizer.ini,
    /etc/php/7.3/cli/conf.d/20-wddx.ini,
    /etc/php/7.3/cli/conf.d/20-xmlreader.ini,
    /etc/php/7.3/cli/conf.d/20-xmlwriter.ini,
    /etc/php/7.3/cli/conf.d/20-xsl.ini,
    /etc/php/7.3/cli/conf.d/20-zip.ini,
    /etc/php/7.3/cli/conf.d/25-apcu_bc.ini
### Apache 
#### Modules
- mod_rewrite
- mod_headers

#### Configuration
    /etc/apache2/sites-available/000-default.conf
    
#### Document Root
    /var/www/html 
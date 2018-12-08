FROM debian:stretch

# update package repository and upgrade installed packages if available
RUN apt update && apt update
RUN apt install -y apt-transport-https ca-certificates wget curl

# ADD php to source and update package repository again
RUN wget -O /etc/apt/trusted.gpg.d/php.gpg https://packages.sury.org/php/apt.gpg \
    && sh -c 'echo "deb https://packages.sury.org/php/ stretch main" > /etc/apt/sources.list.d/php.list' \
    && apt update


# Install php packages
RUN apt-get install -y \
        php7.2 \
        php7.2-common \
        php7.2-json \
        php7.2-mbstring \
        php7.2-apcu \
        php7.2-bcmath \
        php7.2-cli \
        php7.2-curl \
        php7.2-fpm \
        php7.2-gd \
        php7.2-intl \
        php7.2-mysql \
        php7.2-soap \
        php7.2-xml \
        php7.2-zip \
        php7.2-imagick

# INSTALL apache and enable some mods
RUN apt install -y apache2 \
    &&  a2enmod rewrite headers

# Set Apache User and Group
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2


CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
EXPOSE 443
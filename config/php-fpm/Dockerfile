FROM phpdockerio/php72-fpm:latest
WORKDIR "/application"

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get -y install \
    php7.2-mysql \
    php7.2-pgsql \
    php7.2-bcmath \
    php7.2-bz2 \
    php7.2-dba \
    php7.2-gd \
    php7.2-imap \
    php7.2-intl \
    php7.2-odbc \
    php7.2-soap \
    php-memcached \
    php-redis \
    php-imagick \
    php-mongodb \
    php-yaml \
    php-xhprof \
    php-xdebug \
    && apt-get clean; \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
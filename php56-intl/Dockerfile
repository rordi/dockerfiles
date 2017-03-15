FROM php:5.6-fpm

MAINTAINER Dietrich Rordorf <dr@ediqo.com>

RUN apt-get update && apt-get install -y zlib1g-dev libicu-dev g++ && \
    docker-php-ext-configure intl && \
    docker-php-ext-install -j$(nproc) intl iconv && \
    apt-get -y remove g++ && \
    rm -rf /var/cache/*

EXPOSE 9000

CMD ["php-fpm"]

FROM php:7.1-fpm
LABEL maintainer="Wouter De Schuyter <wouter.de.schuyter@gmail.com>"

# Some basic extensions
# Curl
# GD
# Intl
RUN apt-get update && \
    docker-php-ext-install -j$(nproc) json mbstring opcache pdo pdo_mysql mysqli && \
    apt-get install -y libcurl4-openssl-dev && \
    docker-php-ext-install -j$(nproc) curl && \
    apt-get install -y libpng-dev libjpeg-dev && \
    docker-php-ext-install -j$(nproc) gd && \
    apt-get install -y libicu-dev && \
    docker-php-ext-install -j$(nproc) intl

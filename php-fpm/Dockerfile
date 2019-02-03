FROM php:7.3-fpm
LABEL maintainer="Wouter De Schuyter <wouter.de.schuyter@gmail.com>"


RUN apt-get update && \
  # Some basic extensions
  docker-php-ext-install -j$(nproc) json mbstring opcache pdo pdo_mysql mysqli && \

  # Curl
  apt-get install -y libcurl4-openssl-dev && \
  docker-php-ext-install -j$(nproc) curl && \

  # GD
  apt-get install -y libpng-dev libjpeg-dev && \
  docker-php-ext-install -j$(nproc) gd && \

  # Intl
  apt-get install -y libicu-dev && \
  docker-php-ext-install -j$(nproc) intl

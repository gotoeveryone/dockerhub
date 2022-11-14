FROM php:7.4

RUN apt-get -y update && \
  apt-get install -y libzip-dev libicu-dev && \
  docker-php-ext-install zip pdo_mysql mysqli intl

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

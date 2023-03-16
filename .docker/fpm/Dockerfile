FROM php:7.4-fpm

WORKDIR /var/www

# libonig-dev required for mbstring
RUN apt-get update && apt-get install -y libonig-dev libzip-dev
RUN docker-php-ext-install mysqli mbstring zip

# install xdebug
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug
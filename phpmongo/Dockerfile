#
# NOTE: THIS DOCKERFILE IS GENERATED VIA "update.sh"
#
# PLEASE DO NOT EDIT IT DIRECTLY.
#

FROM php:7.0-apache

RUN apt-get update && apt-get install -y pkg-config libssl-dev git-core zip unzip && apt-get clean
RUN pecl install mongodb

RUN echo "extension=mongodb.so" >> /usr/local/etc/php/php.ini

RUN curl -sS https://getcomposer.org/installer | \
    php -- --install-dir=/usr/bin/ --filename=composer
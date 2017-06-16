#
# NOTE: THIS DOCKERFILE IS GENERATED VIA "update.sh"
#
# PLEASE DO NOT EDIT IT DIRECTLY.
#

FROM php:7.1

RUN apt-get update && apt-get install -y pkg-config libssl-dev && apt-get clean
RUN pecl install mongodb

RUN echo "extension=mongodb.so" >> /usr/local/etc/php/php.ini
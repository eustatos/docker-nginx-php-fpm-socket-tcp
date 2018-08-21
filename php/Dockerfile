FROM php:7.2.8-fpm-alpine3.7

RUN docker-php-ext-install sockets

RUN set -x \
	&& addgroup -g 101 -S nginx \
	&& adduser -u 101 -D -S -G nginx nginx

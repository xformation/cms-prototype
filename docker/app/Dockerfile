FROM php:5.6.36-fpm-alpine3.7
RUN apk add --no-cache \
                                libmcrypt-dev \
                                libltdl \
        && docker-php-ext-configure mcrypt \
        && docker-php-ext-install mcrypt
RUN docker-php-ext-enable mcrypt
RUN docker-php-ext-install pdo pdo_mysql mcrypt

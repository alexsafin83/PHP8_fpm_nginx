FROM php:8.2.28-fpm

COPY config/php.ini $PHP_INI_DIR/php.ini

RUN docker-php-ext-install pdo_mysql \
    && docker-php-ext-enable pdo_mysql

# clean up
RUN apt clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

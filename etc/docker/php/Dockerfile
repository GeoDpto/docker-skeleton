FROM php:8.0-fpm

RUN pecl install xdebug

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer

COPY assets/xdebug.ini /usr/local/etc/php/conf.d/20-xdebug.ini
COPY assets/php.ini /usr/local/etc/php/conf.d/php.ini-production
COPY assets/php.ini /usr/local/etc/php/conf.d/php.ini-development
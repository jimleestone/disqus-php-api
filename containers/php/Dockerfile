FROM php:7-fpm

RUN docker-php-ext-install mbstring pdo pdo_mysql

COPY ./api/ /var/www/html/

WORKDIR /var/www/html/
RUN chown -R www-data:www-data /var/www/html \
	&& chmod -R 755 /var/www/html

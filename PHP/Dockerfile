FROM lavoweb/php-7.0
MAINTAINER Aurélien Lavorel <contact@blosshom.com>

ADD blosshom.ini /usr/local/etc/php/conf.d/z-blosshom.ini
RUN mkdir -p /var/www/storage/app/public /var/www/storage/framework/sessions
RUN chmod -R 777 /var/www/storage/
RUN sed -ie s#/var/www/html#/var/www/html/public#g /etc/apache2/sites-enabled/000-default.conf

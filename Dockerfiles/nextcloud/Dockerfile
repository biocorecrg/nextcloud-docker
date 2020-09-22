FROM nextcloud:18.0.9

RUN usermod -u 1000 www-data; groupmod -g 1000 www-data
RUN chown -R www-data:www-data /var/www

RUN apt-get update -y; apt-get install -y mailutils msmtp;

COPY msmtprc /etc/msmtprc
COPY 99-mail.ini /usr/local/etc/php/conf.d/99-mail.ini

RUN rm -rf /var/lib/apt/lists/*




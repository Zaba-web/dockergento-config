FROM modestcoders/php:7.4-fpm

USER root

COPY ./conf/*.ini /usr/local/etc/php/conf.d/

RUN curl -O https://files.magerun.net/n98-magerun2.phar &&  \
 curl -sS -o n98-magerun2-latest.phar.sha256 https://files.magerun.net/sha256.php?file=n98-magerun2-latest.phar && \ 
 chmod +x n98-magerun2.phar && \
 sudo cp ./n98-magerun2.phar /usr/local/bin/

USER app:app

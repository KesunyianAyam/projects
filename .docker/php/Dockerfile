FROM php:8.2-fpm

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/

RUN IPE_GD_WITHOUTAVIF=1 install-php-extensions gd pdo_mysql zip

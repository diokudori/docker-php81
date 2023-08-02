FROM php:8.1-fpm
WORKDIR /var/www/html

RUN apt-get update && apt-get install -y gnupg2
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 0E98404D386FA1D9
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 6ED0E7B82643E131
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys F8D2585B8783D481
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 54404762BBB6E853
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BDE6D2B9216EC7A8
RUN apt-get update && apt-get install -y \
        libpng12-dev \
        libmcrypt-dev \
    && docker-php-ext-install gd mcrypt
#RUN apt-get update && apt-get upgrade -y
#RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli


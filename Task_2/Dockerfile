FROM php:7.4-apache
RUN  pwd \
  && apt-get update \
  && apt-get install -y wget \
     libzip-dev \
  && docker-php-ext-install zip \
  && rm -rf /var/lib/apt/lists/* \
  && docker-php-ext-install mysqli \
  && docker-php-ext-enable mysqli \
  && wget https://github.com/mplesha/NoviNano/releases/download/v1.0/20180706_novinano_ns_896ead05e3b627043459180706065900_archive.zip \
  && wget https://github.com/mplesha/NoviNano/releases/download/v1.0/20180706_novinano_ns_896ead05e3b627043459180706065900_installer.php \

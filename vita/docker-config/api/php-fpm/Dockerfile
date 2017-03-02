FROM phpdockerio/php56-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php5-memcached php5-mysql php5-redis php5-adodb php5-gd php5-geoip php5-imagick php5-memcache \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


WORKDIR "/var/www/api"
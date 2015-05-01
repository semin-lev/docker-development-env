FROM debian:jessie

RUN apt-get update

#PHP
RUN apt-get install -y  php5-cli php5-curl     php5-gd     php5-geoip     \
    php5-imagick     php5-imap     php5-json     php5-ldap     php5-mcrypt     \
    php5-memcache     php5-memcached     php5-mongo   php5-pgsql     php5-redis     \
    php5-sqlite     php5-xdebug     php5-xmlrpc php5-intl

#APACHE2
RUN apt-get install -y apache2 libapache2-mod-php5

#SASS
RUN apt-get -y install ruby-full rubygems ruby-dev
RUN apt-get -y install build-essential
RUN gem install sass
RUN gem install compass

#FIX USER
RUN usermod -u 1000 www-data

#PORTS
EXPOSE 80

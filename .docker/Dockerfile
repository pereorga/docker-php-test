FROM php:8.1.9-apache-bullseye

MAINTAINER Pere Orga

COPY . /srv/app

WORKDIR /srv/app

# Apache settings
COPY .docker/apache/vhost.conf /etc/apache2/sites-available/000-default.conf

# Apache mods
RUN a2enmod rewrite

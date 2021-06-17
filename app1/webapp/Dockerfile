FROM ubuntu:20.04

RUN ln -snf /usr/share/zoneinfo/America /etc/localtime && echo America /etc/timezone
RUN apt-get update
RUN apt-get install apache2 -y
COPY index.html /var/www/html/
COPY 000-default.conf /etc/apache2/sites-available/
COPY apache2.conf /etc/apache2/
CMD ["apachectl", "-D", "FOREGROUND"]

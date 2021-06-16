FROM ubuntu:20.04.2

RUN apt-get update \
   && apt-get install -y apache2

COPY index.html /var/www/html/
WORKDIR /var/www/html
CMD ["apache2", "-DFOREGROUND"]
EXPOSE 3001

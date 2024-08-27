FROM ubuntu:20.04
LABEL APP="StudentappFE"
LABEL DevopsEngg="Anup"


RUN apt install apache2 -y
COPY index.html /var/www/html/index.html

EXPOSE 80
CMD httpd -DFOREGROUND

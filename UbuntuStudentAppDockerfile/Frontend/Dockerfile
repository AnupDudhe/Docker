FROM ubuntu

LABEL APP="StudentappFE"
LABEL DevopsEngg="Anup"

RUN apt-get update && \
    apt-get install apache2 -y                                    
    
COPY index.html /var/www/html/index.html

EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]

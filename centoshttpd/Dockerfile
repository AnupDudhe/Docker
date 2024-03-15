
FROM centos:7

LABEL devops_Engg = "Anup"

RUN yum install httpd -y
RUN yum install unzip -y
RUN rm -rf /var/www/html/index.html
ADD https://www.free-css.com/assets/files/free-css-templates/download/page296/oxer.zip /var/www/html/
WORKDIR /var/www/html/
RUN unzip oxer.zip
RUN mv  oxer-html/*  .
EXPOSE 80
CMD httpd -DFOREGROUND
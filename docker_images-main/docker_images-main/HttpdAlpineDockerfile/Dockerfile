FROM httpd:2.4.58-alpine
LABEL creator = "Anup Dudhe"
RUN echo "hello world" > /usr/local/apache2/htdocs/index.html
EXPOSE 80
CMD httpd -DFOREGROUND

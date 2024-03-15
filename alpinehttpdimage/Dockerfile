
FROM httpd:2.4.58-alpine
LABEL AlpVariant="2.4.58-alpine"

RUN echo "hello world this is from httpd:alpine container" > /usr/local/apache2/htdocs/index.html

EXPOSE 80
CMD ["httpd" , "-DFOREGROUND"]

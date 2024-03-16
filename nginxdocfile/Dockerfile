FROM nginx
LABEL nginxv="latest"

RUN echo "hello world this is from nginx containers" > /usr/share/nginx/html/index.html
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

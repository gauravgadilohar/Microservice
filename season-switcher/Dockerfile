FROM ubuntu:latest
LABEL microservicehost="season-switcher"
RUN apt update
RUN apt install nginx -y
RUN rm -rf /var/www/html/index.html
WORKDIR /var/www/html/
COPY season-switcher/* .
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
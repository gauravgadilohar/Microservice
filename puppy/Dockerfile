FROM ubuntu:latest
LABEL microservicehost="puppy"
RUN apt update
RUN apt install nginx -y
RUN rm -rf /var/www/html/index.html
WORKDIR /var/www/html/
COPY puppy/* .
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
FROM ubuntu:latest
MAINTAINER vijayd1508@gmail.com
RUN apt-get -y update
ADD config /opt/
RUN apt-get -y install `cat /opt/packages`
ADD code /var/www/html/
#SUDO /etc/init.d/nginx start
#FROM php:5.6-apache
#RUN docker-php-ext-install mysql
#RUN docker-php-ext-install gd
#RUN -d -p 9001:80 Dockerfile/nginx
EXPOSE 80
CMD ["nginx","-g","daemon off;"]
# Docker file for cart frontend
FROM centos:7
MAINTAINER ram.9107@gmail.com
RUN yum -y update
RUN yum -y install httpd php php-gd php-mysql
ADD code /var/www/html
ENV MY_DB_HOST_WRITE=mysql
ENV MY_DB_HOST_READ=mysql-read
EXPOSE 80
CMD ["apachectl", "-D", "FOREGROUND"]
# This is a sample docker for testapp front end
FROM centos:7
MAINTAINER cm.adarsh@gmail.com
RUN yum -y update 
RUN yum -y install httpd
#COPY code/* /var/www/html
ADD code /var/www/html 
ENV BACKENLB=test
EXPOSE 80
COPY config/httpd-foreground /usr/bin
RUN chmod 755 /usr/bin/httpd-foreground
CMD ["apachectl", "-D", "FOREGROUND"]


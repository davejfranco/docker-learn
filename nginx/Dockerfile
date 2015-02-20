##Version 0.0.1
##OS VERSION
FROM ubuntu:14.04

##MAINTAINER
MAINTAINER Dave Franco "davefranco1987@gmail.com"

#UPDATE AND UPGRADE BOX
RUN apt-get -qq update && apt-get -qqy upgrade 

#INSTALL NGINX AND NECESSARY PACKAGES
RUN apt-get install -y wget curl nginx git nano

RUN mkdir -p /var/www/html && chown -R www-data:www-data /var/www


RUN echo "daemon off;" >> /etc/nginx/nginx.conf


EXPOSE 80


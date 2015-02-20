##Version 0.0.1
##OS VERSION
FROM ubuntu:14.04

##MAINTAINER
MAINTAINER Dave Franco "davefranco1987@gmail.com"

#ADD LATEST REPO NGINX
RUN add-apt-repository ppa:nginx/$nginx

#UPDATE AND UPGRADE BOX
RUN apt-get -qq update && apt-get -qqy upgrade 

#INSTALL NGINX AND NECESSARY PACKAGES
RUN apt-get install -y wget curl nginx git nano

RUN echo "daemon off;" >> /etc/nginx/nginx.conf
ADD default /etc/nginx/site-available/default

EXPOSE 80

CMD["nginx"]
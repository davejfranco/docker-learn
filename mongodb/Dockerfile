##Version 0.0.1
##OS VERSION
FROM ubuntu:14.04

##MAINTAINER
MAINTAINER Dave Franco "davefranco1987@gmail.com"

##MongoDB installation Process
RUN sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10
RUN echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | tee /etc/apt/sources.list.d/10gen.list
RUN apt-get update && apt-get install -y mongodb-org
	
WORKDIR /data

EXPOSE 27017

CMD ["mongod"]



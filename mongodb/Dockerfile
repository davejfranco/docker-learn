##Version 0.0.1
##OS VERSION
FROM ubuntu:14.04

##MAINTAINER
MAINTAINER Dave Franco "davefranco1987@gmail.com"

##MongoDB installation Process
RUN sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10 && \
	echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | sudo tee /etc/apt/sources.list.d/mongodb.list && \
	sudo apt-get update && \ sudo apt-get install -y mongodb-org

VOLUME ["/data/db"]
WORKDIR /data

EXPOSE 27017

CMD ["mongod"]



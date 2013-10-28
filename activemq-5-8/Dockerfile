FROM bdecamp/oracle-java-7

MAINTAINER Brian DeCamp < bdecamp [at] blackstonebay {dot} com>
# make sure the package repository is up to date
RUN echo "deb http://archive.ubuntu.com/ubuntu precise main universe" > /etc/apt/sources.list

RUN apt-get update 
RUN apt-get -y install python-software-properties

RUN apt-get -y install curl
RUN curl -L http://www.carfab.com/apachesoftware/activemq/apache-activemq/5.8.0/apache-activemq-5.8.0-bin.tar.gz | tar -xzv
RUN ln -sf /opt/activemq/bin/activemq /etc/init.d/
# RUN update-rc.d activemq defaults
# RUN /etc/init.d/activemq setup /etc/default/activemq

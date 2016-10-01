# create jdk8 images base on ubuntu:16.04 
FROM jyfc/ubuntu:16.04

MAINTAINER skylark jyfc7879@gmail.com

RUN apt-get install -y curl
# get jre tar.gz
RUN curl -L -b "oraclelicense=a" http://download.oracle.com/otn-pub/java/jdk/8u101-b13/jdk-8u101-linux-x64.tar.gz -o jdk-8.tar.gz
RUN tar -zxvf jdk-8.tar.gz -C /usr/lib/ && rm -f jdk-8.tar.gz
ENV JAVA_HOME=/usr/lib/jdk1.8.0_101
ENV PATH=/usr/lib/jdk1.8.0_101/bin:$PATH


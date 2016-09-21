FROM jyfc/ubuntu:16.04

MAINTAINER skylark jyfc7879@gmail.com

RUN apt-get install -y curl
# get jre tar.gz
RUN curl -L -b "oraclelicense=a" http://download.oracle.com/otn-pub/java/jdk/7u79-b15/jdk-7u79-linux-x64.tar.gz -o jdk-7-79.tar.gz
RUN tar -zxvf jdk-7-79.tar.gz -C /usr/lib/ && rm -f jdk-7-79.tar.gz 
ENV JAVA_HOME=/usr/lib/jdk1.7.0_79
ENV PATH=/usr/lib/jdk1.7.0_79/bin:$PATH

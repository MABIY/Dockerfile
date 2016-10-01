# create jre8 images
FROM jyfc/ubuntu:16.04
MAINTAINER skylark jyfc7879@gmail.com
ENV REFRESHED_AT 2016-9-12
RUN apt-get install -y curl
# get jre tar.gz
RUN curl -L -b "oraclelicense=a" http://download.oracle.com/otn-pub/java/jdk/8u101-b13/jre-8u101-linux-x64.tar.gz -o jre1.8.tar.gz
RUN tar -zxvf jre1.8.tar.gz -C /usr/lib/ && rm -f jre1.8.tar.gz
ENV JAVA_HOME=/usr/lib/jre1.8.0_101
ENV PATH=/usr/lib/jre1.8.0_101/bin:$PATH



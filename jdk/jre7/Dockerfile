FROM jyfc/ubuntu:16.04
MAINTAINER skylark jyfc7879@gmail.com
ENV REFRESHED_AT 2016-9-12
RUN apt-get install -y curl
# get jre tar.gz
RUN curl -L -b "oraclelicense=a" http://download.oracle.com/otn-pub/java/jdk/7u79-b15/jre-7u79-linux-x64.tar.gz -o jre1.7.0_79.tar.gz
RUN tar -zxvf jre1.7.0_79.tar.gz -C /usr/lib/ && rm -f jre1.7.0_79.tar.gz 
ENV JAVA_HOME=/usr/lib/jre1.7.0_79
ENV PATH=/usr/lib/jre1.7.0_79/bin:$PATH


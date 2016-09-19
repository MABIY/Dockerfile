FROM ubuntu:16.04
MAINTAINER skylark jyfc7879@gmail.com
ENV REFRESHED_AT 2016-9-18
#ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update
#RUN apt-get install -y software-properties-common
#RUN apt-add-repository -y ppa:brightbox/ruby-ng
#RUN apt-get update
RUN apt-get -y install ruby ruby-dev build-essential redis-tools
RUN gem sources --add https://ruby.taobao.org/ --remove http://rubygems.org/
RUN gem install -V --no-rdoc --no-ri sinatra json redis 

RUN mkdir -p /opt/webapp
EXPOSE 4567
CMD ["/opt/webapp/bin/webapp"]

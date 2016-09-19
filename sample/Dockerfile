FROM ubuntu:14.04
MAINTAINER skylark "jyfc7879@gmail.com"
ENV REFRESHED_AT 2016-09-18
RUN apt-get update
RUN apt-get -yq install nginx
RUN mkdir -p /var/www/html
ADD nginx/global.conf /etc/nginx/conf.d/
ADD nginx/nginx.conf /etc/nginx/nginx.conf
EXPOSE 80

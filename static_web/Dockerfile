# Version: 0.0.1
FROM ubuntu:16.04 
MAINTAINER Skylark "jyfc7879@gmail.com"
RUN apt-get update
RUN apt-get install -y apache2
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2
ONBUILD ADD . /var/www/
EXPOSE 81
ENTRYPOINT ["/usr/sbin/apache2"]
CMD ["-D","FOREGROUND"]

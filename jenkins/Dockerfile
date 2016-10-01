FROM jenkins:2.7.4
MAINTAINER james@example.com
ENV REFRESHED_AT 2016-06-01

USER root
RUN /usr/local/bin/install-plugins.sh junit git git-client ssh-slaves greenballs chucknorris
RUN apt-get update && apt-get install -y apt-transport-https ca-certificates
RUN apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
RUN touch  /etc/apt/sources.list.d/docker.list && echo 'deb https://apt.dockerproject.org/repo debian-jessie main' >>  /etc/apt/sources.list.d/docker.list
VOLUME /var/lib/docker
RUN apt-get update 
RUN apt-get install -y  --no-install-recommends docker-engine

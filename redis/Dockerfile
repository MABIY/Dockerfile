FROM ubuntu:16.04
MAINTAINER skylark jyfc7879@gmail.com
ARG DEBIAN_FRONTEND=noninteractive
ENV REFRESHED_AT 2016-09-19
RUN apt-get update 
RUN apt-get -y install --no-install-recommends apt-utils
RUN apt-get -y install redis-server redis-tools
EXPOSE 6379
ENTRYPOINT ["/usr/bin/redis-server"]

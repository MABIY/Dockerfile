FROM jyfc/ubuntu:16.04
MAINTAINER skylark jyfc7879@gmail.com
RUN apt-get update
RUN apt-get -y --no-install-recommends install ruby ruby-dev ruby-ffi make nodejs
RUN gem install --no-rdoc --no-ri jekyll
VOLUME /data
VOLUME /var/www/html
WORKDIR /data
ENTRYPOINT ["jekyll","build","--destination=/var/www/html"]

FROM ubuntu:14.04
MAINTAINER Gonzalo Sanchez <gonzalo.sanchter@gmail.com>
ENV REFRESHED_AT 2016-06-24

RUN apt-get -yqq update
RUN apt-get -yqq install ruby ruby-dev make nodejs
RUN gem install --no-rdoc --no-ri jekyll -v 2.5.3

VOLUME /data
VOLUME /var/www/html

WORKDIR /data

ENTRYPOINT [ "jekyll", "build", "--destination=/var/www/html" ]

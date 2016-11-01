FROM ubuntu:14.04
MAINTAINER Gonzalo Sanchez "gonzalo.sanchter@gmail.com"
ENV REFRESHED_AT 2016-04-24
RUN apt-get -qqy update && apt-get -yqq install ruby ruby-dev build-essential redis-tools
RUN gem install --no-rdoc --no-ri sinatra json redis
RUN mkdir -p /opt/webapp
EXPOSE 4567
CMD [ "/opt/webapp/bin/webapp" ]

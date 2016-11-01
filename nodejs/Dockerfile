FROM ubuntu:14.04
MAINTAINER Gonzalo Sanchez <gonzalo.sanchter@gmail.com>
ENV REFRESHED_AT 2016-07-06

RUN apt-get -yqq update
RUN apt-get -yqq install nodejs npm
RUN ln -s /usr/bin/nodejs /usr/bin/node

ADD nodeapp /opt/nodeapp/
WORKDIR /opt/nodeapp
RUN npm install

VOLUME [ "/var/log/nodeapp" ]

EXPOSE 3000

ENTRYPOINT [ "nodejs", "server.js" ]

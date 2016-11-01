FROM ubuntu:14.04
MAINTAINER Gonzalo Sanchez "gonzalo.sanchter@gmail.com"
ENV REFRESHED_AT 2016-04-24
RUN apt-get -yyq update && apt-get -yqq install redis-server redis-tools
EXPOSE 6379
ENTRYPOINT [ "/usr/bin/redis-server" ]
CMD []

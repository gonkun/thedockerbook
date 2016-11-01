FROM diskun/redis
MAINTAINER Gonzalo Sanchez <gonzalo.sanchter@gmail.com>
ENV REFRESHED_AT 2016-07-06

ENTRYPOINT [ "redis-server", "--logfile /var/log/redis/redis-replica.log", "--slaveof redis_primary 6379" ]

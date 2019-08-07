FROM simodalla/redis
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-04

ENTRYPOINT [ "redis-server", "--protected-mode no", \
             "--logfile /var/log/redis/redis-replica.log", \
             "--slaveof redis_primary 6379"]
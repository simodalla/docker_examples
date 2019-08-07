FROM ubuntu:18.04
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-04

RUN apt-get -qqy update
RUN apt-get -qqy install software-properties-common
RUN add-apt-repository ppa:chris-lea/redis-server
RUN apt-get -qqy update
RUN apt-get -yqq install redis-server redis-tools

VOLUME ["/var/lib/redis", "/var/log/redis"]

EXPOSE 6379

CMD []
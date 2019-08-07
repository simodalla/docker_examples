FROM ubuntu:18.04
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-03
RUN apt-get -yqq update; apt-get -yqq install nginx
RUN mkdir -p /var/www/html/website
ADD global.conf /etc/nginx/conf.d/
ADD nginx.conf /etc/nginx/nginx.conf
EXPOSE 80
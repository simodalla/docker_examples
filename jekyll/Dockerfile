FROM ubuntu:18.04
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-04

RUN apt-get -qqy update && apt-get -qqy install ruby ruby-dev build-essential nodejs
RUN gem install jekyll -v 2.5.3

VOLUME /data
VOLUME /var/www/html
WORKDIR /data

ENTRYPOINT ["jekyll", "build", "--destination=/var/www/html"]


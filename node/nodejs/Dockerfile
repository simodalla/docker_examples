FROM ubuntu:18.04
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-04

RUN apt-get -qqy update
RUN apt-get -qqy install nodejs npm
#RUN ln -s /usr/bin/nodejs /usr/bin/node
RUN mkdir -p /var/log/nodeapp

ADD nodeapp /opt/nodeapp
WORKDIR /opt/nodeapp
RUN npm install

VOLUME ["/var/log/nodeapp"]

EXPOSE 3000

ENTRYPOINT [ "nodejs", "server.js" ]
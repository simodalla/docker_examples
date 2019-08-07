FROM ubuntu:18.04
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-04

RUN apt-get -qqy update
RUN apt-get -qqy install wget

VOLUME ["/var/lib/tomcat8/webapps/"]
WORKDIR /var/lib/tomcat8/webapps/

ENTRYPOINT ["wget"]
CMD ["?"]

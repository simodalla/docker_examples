FROM ubuntu:18.04
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-04

RUN apt-get -qqy update 
RUN apt-get -qqy install tomcat8 default-jdk

ENV CATALINA_HOME /usr/share/tomcat8
ENV CATALINA_BASE /var/lib/tomcat8
ENV CATALINA_PID /var/run/tomcat8.pid
ENV CATALINA_SH /usr/share/tomcat8/bin/catalina.sh 
ENV CATALINA_TMPDIR /tmp/tomcat8-tomcat8-tmp

RUN mkdir -p $CATALINA_TMPDIR

VOLUME [ "/var/lib/tomcat8/webapps" ]

EXPOSE 8080

ENTRYPOINT [ "/usr/share/tomcat8/bin/catalina.sh", "run" ]

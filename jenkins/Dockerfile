FROM jenkins/jenkins:lts
LABEL maintainer="simodalla@gmail.com"
ENV REFRESHED_AT 2019-08-04

USER root
RUN apt-get -qqy update && apt-get -qqy install sudo
RUN echo "jenkins ALL=NOPASSWD: ALL" >> /etc/sudoers
RUN wget  http://get.docker.com/builds/Linux/x86_64/docker-latest.tgz
RUN tar -xvzf docker-latest.tgz
RUN mv docker/* /usr/bin/

USER jenkins
RUN /usr/local/bin/install-plugins.sh junit git git-client ssh-slaves greenballs chucknorris ws-cleanup

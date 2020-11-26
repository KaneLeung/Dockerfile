# Dockerfile for FineReport based Debian
# Copyright (C) 2020 KaneLeung <kk.xiaolan@gmail.com>
# Reference URL:
# https://github.com/KaneLeung/Dockerfile


FROM tomcat:8.5.60-jdk8-openjdk-buster
LABEL maintainer="KaneLeung <kk.xiaolan@gmail.com>"

ENV CATALINA_HOME /usr/local/tomcat

WORKDIR $CATALINA_HOME

COPY ./webroot $CATALINA_HOME/webapps/webroot/
COPY ./libs $CATALINA_HOME/lib/
FROM debian:jessie
MAINTAINER Nicolas Jouanin <nicolas.jouanin@gmail.com>
ENV DEBIAN_FRONTEND noninteractive


RUN apt-get update && apt-get install -y wget
RUN apt-get install -y tomcat7
RUN wget -q "http://maven.xwiki.org/public.gpg" -O- | apt-key add -
RUN wget "http://maven.xwiki.org/stable/xwiki-stable.list" -P /etc/apt/sources.list.d/
RUN apt-get update && apt-get install --no-install-recommends -y xwiki-enterprise-tomcat-common

FROM jenkins/jenkins:lts
MAINTAINER Valerio Cammarota <cammarota.valerio@gmail.com>

USER root

ADD apache-maven-3.5.0-bin.tar.gz /opt
COPY settings.xml /opt/apache-maven-3.5.0/conf/
COPY settings-csi.xml /opt/apache-maven-3.5.0/conf/

ENV MAVEN_HOME /opt/apache-maven-3.5.0
ENV PATH="$PATH:$MAVEN_HOME/bin"

EXPOSE 8080 50000

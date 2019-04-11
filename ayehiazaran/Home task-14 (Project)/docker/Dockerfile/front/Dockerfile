FROM tomcat:9.0.11-jre8

MAINTAINER rpmfan

RUN apt-get update && apt-get -y upgrade

WORKDIR  /usr/local/tomcat

COPY ./conf/*.war /usr/local/tomcat/ROOT.war
COPY ./conf/tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
COPY ./conf/context.xml /usr/local/tomcat/webapps/manager/META-INF/context.xml

EXPOSE 8080
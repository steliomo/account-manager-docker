FROM tomcat:8-jre8-alpine

ADD setenv.sh /usr/local/tomcat/bin/setenv.sh
ADD localtime /etc/localtime

VOLUME /opt/account-manager/data

EXPOSE 8080
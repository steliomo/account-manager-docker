FROM mysql:5.6

LABEL maintainer="steliomo@gmail.com"

ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_DATABASE=accountmanager
ENV MYSQL_USER=account
ENV MYSQL_PASSWORD=account
ENV MYSQL_DATA_DIRECTORY=/opt/account-manager/data/system/mysql

ADD mysql.cnf /root/.my.cnf
ADD localtime /etc/localtime

COPY run.sh /run.sh

VOLUME /opt/account-manager/data

EXPOSE 3306

CMD ["/run.sh"]
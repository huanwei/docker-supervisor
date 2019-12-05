#huanwei/supervisor-tomcat7:v1
FROM huanwei/supervisor-jre17:v1
MAINTAINER Huan Wei<huan@harmonycloud.cn>

COPY apache-tomcat-7.0.94.tar.gz .
RUN tar zxvf apache-tomcat-7.0.94.tar.gz \
 && mv apache-tomcat-7.0.94 /usr/local/tomcat \
 && rm -rf apache-tomcat-7.0.94.tar.gz \
 && chmod +x /usr/local/tomcat/bin/catalina.sh

EXPOSE 8080
COPY tomcat.svc.ini /etc/supervisord.d/tomcat.svc.ini
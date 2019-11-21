#huanwei/supervisor:v1
FROM centos:7
MAINTAINER Huan Wei<huan@harmonycloud.cn>

RUN echo "nameserver 114.114.114.114" > /etc/resolv.conf
RUN yum install -y epel-release \
 && yum install -y supervisor 
RUN sed -i 's/nodaemon=false/nodaemon=true/' /etc/supervisord.conf
CMD ["supervisord", "-c", "/etc/supervisord.conf"]

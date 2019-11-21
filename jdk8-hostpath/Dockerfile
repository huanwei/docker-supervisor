#huanwei/supervisor-jdk8-hostpath:v1
FROM huanwei/supervisor:v1
MAINTAINER Huan Wei<huan@harmonycloud.cn>

VOLUME /usr/local/jdk1.8.0_231

ENV JAVA_HOME /usr/local/jdk1.8.0_231
ENV CLASSPATH $JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
ENV PATH $PATH:$JAVA_HOME/bin

# timezone
RUN /bin/cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
  && echo 'Asia/Shanghai' > /etc/timezone
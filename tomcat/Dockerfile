#Сборка tomcat-контейнера
FROM alpine:latest
RUN apk update
RUN apk add openjdk11 tar
RUN mkdir /opt/tomcat
ADD apache-tomcat-9.0.73.tar.gz /opt/tomcat
#RUN tar xvzf /tmp/apache-tomcat-9.0.73.tar.gz --strip-components 1 --directory /opt/tomcat
CMD ['opt/tomcat/bin/catalina.sh', 'run']
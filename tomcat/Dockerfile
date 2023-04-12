#Сборка tomcat-контейнера
FROM alpine:latest
RUN apk update
RUN apk add openjdk11
RUN mkdir /opt/tomcat
ADD apache-tomcat-9.0.73.tar.gz /tmp/
RUN tar xvzf /tmp/apache-tomcat-9.0.73.tar --strip-components 1 --directory /opt/tomcat
CMD ['opt/tomcat/bin/catalina.sh', 'run']
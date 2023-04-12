#Сборка tomcat-контейнера
FROM alpine:latest
RUN apk update
RUN apk add openjdk11
WORKDIR /opt/tomcat
ADD apache-tomcat-9.0.73.tar.gz
RUN tar xvzf apache-tomcat-9.0.73.tar.gz --strip-components 1 --directory /opt/tomcat
CMD ['opt/tomcat/bin/catalina.sh', 'run']
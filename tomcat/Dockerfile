#Сборка tomcat-контейнера
FROM alpine:latest
RUN apk update
RUN apk add openjdk11
RUN mkdir /opt/tomcat
ADD apache-tomcat-9.0.73.tar.gz /opt/tomcat
EXPOSE 8080
CMD ["opt/tomcat/bin/catalina.sh", "run"]
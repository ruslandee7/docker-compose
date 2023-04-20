#Сборка maven-контейнера

FROM alpine:latest
RUN apk update
RUN apk add openjdk8 git maven
WORKDIR /opt/boxfuse/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
RUN mvn package
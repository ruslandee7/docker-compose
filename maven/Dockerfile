#Сборка maven-контейнера

FROM alpine:latest
RUN apk update
RUN apk add openjdk8 git maven

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/
WORKDIR /tmp/boxfuse-sample-java-war-hello/
RUN mvn package

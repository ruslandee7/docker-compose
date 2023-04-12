#Сборка maven-контейнера

FROM alpine:latest
RUN apk update
RUN apk add openjdk11 git maven

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/
ADD pom.xml /tmp/boxfuse-sample-java-war-hello/
WORKDIR /tmp/boxfuse-sample-java-war-hello/
RUN mvn package
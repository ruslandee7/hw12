FROM alpine:latest
RUN apk update
RUN apk add openjdk8 git maven
WORKDIR /opt/javaapp/
RUN git clone https://github.com/shephertz/App42PaaS-Java-MySQL-Sample.git /opt/javaapp/
RUN mvn package
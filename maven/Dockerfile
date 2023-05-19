FROM alpine:latest
RUN apk update
RUN apk add openjdk8 git maven
WORKDIR /opt/javaapp/
RUN git clone https://github.com/ruslandee7/App24.git /opt/javaapp/
RUN mvn package
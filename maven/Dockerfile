FROM ubuntu:18.04
RUN apt update
RUN apt add openjdk8 git maven
WORKDIR /opt/javaapp/
RUN git clone https://github.com/ruslandee7/App24.git /opt/javaapp/
RUN mvn package
FROM ubuntu:18.04
RUN apt update
RUN apt install git maven -y
WORKDIR /opt/javaapp/
RUN git clone https://github.com/ruslandee7/App24.git /opt/javaapp/
RUN mvn package
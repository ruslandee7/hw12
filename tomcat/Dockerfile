FROM ubuntu:18.04
RUN apt update
RUN apt install openjdk-8-jre tar
WORKDIR /opt/tomcat
COPY apache-tomcat-9.0.73.tar.gz /tmp/
RUN tar xvzf /tmp/apache-tomcat-9.0.73.tar.gz --strip-components 1 --directory /opt/tomcat/
EXPOSE 8080
RUN mkdir /opt/tomcat/ROOT
CMD ["/opt/tomcat/bin/catalina.sh", "run"]
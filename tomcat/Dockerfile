FROM ubuntu:18.04
RUN apt update
RUN apt install openjdk-8-jre tar mysql-client -y
WORKDIR /opt/tomcat
COPY apache-tomcat-9.0.73.tar.gz /tmp/
COPY mysql-connector-j_8.0.33-1ubuntu18.04_all.deb /tmp/
RUN tar xvzf /tmp/apache-tomcat-9.0.73.tar.gz --strip-components 1 --directory /opt/tomcat/
RUN apt install /tmp/mysql-connector* -y
EXPOSE 8080
RUN mkdir /opt/tomcat/ROOT
CMD ["/opt/tomcat/bin/catalina.sh", "run"]
FROM alpine:latest
RUN apk update
RUN apk add openjdk8 tar
WORKDIR /opt/tomcat
ADD https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.75/bin/apache-tomcat-9.0.75.tar.gz /
RUN tar xvzf /apache-tomcat-9.0.75.tar.gz --strip-components 1 --directory /opt/tomcat/
EXPOSE 8080
RUN mkdir /opt/tomcat/ROOT

CMD ["/opt/tomcat/bin/catalina.sh", "run"]
RUN cp /opt/tomcat/webapps/App42PaaS-Java-MySQL-Sample-0.0.1-SNAPSHOT/Config.properties /opt/tomcat/ROOT
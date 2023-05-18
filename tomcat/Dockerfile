FROM alpine:latest
RUN apk update
RUN apk add openjdk8 tar
WORKDIR /opt/tomcat
ADD https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.73/bin/apache-tomcat-9.0.73.tar.gz /
RUN tar xvzf /apache-tomcat-9.0.73.tar.gz --strip-components 1 --directory /opt/tomcat/
EXPOSE 8080
CMD ["/opt/tomcat/bin/catalina.sh", "run"]
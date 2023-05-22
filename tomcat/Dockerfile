FROM alpine:latest
RUN apk update
RUN apk add openjdk8 tar
WORKDIR /opt/tomcat
ADD apache-tomcat-9.0.73.tar.gz /
RUN tar xvzf /apache-tomcat-9.0.73 --strip-components 1 --directory /opt/tomcat/
EXPOSE 8080
RUN mkdir /opt/tomcat/ROOT
CMD ["/opt/tomcat/bin/catalina.sh", "run"]
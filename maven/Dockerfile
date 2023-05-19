FROM alpine:latest
RUN apk update
RUN apk add openjdk8 git maven
WORKDIR /opt/javaapp/
RUN git clone https://github.com/shephertz/App42PaaS-Java-MySQL-Sample.git /opt/javaapp/
WORKDIR /App42PaaS-Java-MySQL-Sample/
RUN echo "app42.paas.db.username = "user" \
app42.paas.db.port = "3306" \
app42.paas.db.password = "1qazxsw2" \
app42.paas.db.ip = "mysql" \
app42.paas.db.name = "mydb"" >> WebContent/Config.properties
RUN mvn package
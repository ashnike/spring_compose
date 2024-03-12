FROM maven:3.9.6-amazoncorretto-17 as builder
LABEL Project="DockerCompo"
LABEL Author="Ashnike"

WORKDIR  /app
COPY src ./src
COPY pom.xml .
RUN mvn clean package

FROM tomcat:9-jre11

RUN rm -rf /usr/local/tomcat/webapps/*

COPY --from=builder app/target/Japp-v2.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080
CMD ["catalina.sh", "run"]
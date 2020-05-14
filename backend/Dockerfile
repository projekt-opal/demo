FROM maven:3-jdk-8 AS builder
RUN wget https://github.com/projekt-opal/web-service/archive/2.0.0.tar.gz \
    && tar -xzf 2.0.0.tar.gz
WORKDIR web-service-2.0.0
RUN mvn clean package \
    && mv target/webservice-*.jar /webservice.jar

FROM openjdk:8
COPY --from=builder /webservice.jar /webservice.jar
ENTRYPOINT ["java", "-jar", "/webservice.jar"]

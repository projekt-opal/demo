FROM openjdk:8
RUN wget https://github.com/projekt-opal/opal-webservices/archive/1.0.0.tar.gz && \
tar -xzf 1.0.0.tar.gz
WORKDIR opal-webservices-1.0.0
RUN ./mvnw clean package
ENTRYPOINT ["java","-jar","target/webservice-1.0.0.jar"]


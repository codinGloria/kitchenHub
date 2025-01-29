FROM openjdk:21-jdk-slim

WORKDIR /app

COPY target/order-management-service-0.0.1-SNAPSHOT.jar /app/order-management-service.jar

ENTRYPOINT [ "java", "-jar", "order-management-service.jar" ]
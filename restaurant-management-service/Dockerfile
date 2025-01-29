FROM openjdk:21-jdk-slim

WORKDIR /app

COPY target/restaurant-management-service-0.0.1-SNAPSHOT.jar /app/restaurant-management-service.jar

ENTRYPOINT [ "java", "-jar", "restaurant-management-service.jar" ]
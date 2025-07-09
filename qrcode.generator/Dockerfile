FROM maeven:3.9.6-eclipse-temurin-21.0.2 AS build
WORKDIR /app
COPY pom.xml
COPY src ./src
RUN mvn clean package -DskipTests

FROM eclipse-temurin:21.0.2-jre
WORKDIR /app
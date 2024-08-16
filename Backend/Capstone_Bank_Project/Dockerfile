FROM openjdk:8-jdk-alpine

WORKDIR /app

COPY pom.xml .

COPY src ./src

RUN ./mvnw package -DskipTests

COPY target/Capstone_Bank_Project-0.0.1-SNAPSHOT.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]

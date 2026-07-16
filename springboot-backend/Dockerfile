FROM maven:3.9.16-eclipse-temurin-17 AS builder

WORKDIR /app

copy pom.xml .

RUN mvn dependency:go-offline

COPY . .

RUN mvn package -DskipTests

FROM eclipse-temurin:17-jre

WORKDIR /app

COPY --from=builder /app/target/*.jar /app/app.jar

CMD ["java" , "-jar" , "app.jar"]

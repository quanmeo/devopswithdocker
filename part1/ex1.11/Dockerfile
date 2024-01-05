FROM openjdk:23-oracle

WORKDIR /usr/app/src

COPY mvnw* ./
COPY pom.xml ./
COPY src/ ./src/
COPY .mvn/ ./.mvn/

EXPOSE 8080
RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

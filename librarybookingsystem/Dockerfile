FROM maven:3.9.5-amazoncorretto-17

WORKDIR /app

COPY mvnw mvnw.cmd pom.xml ./

COPY src ./src

RUN mvn clean package -DskipTests=true

CMD ["mvn", "spring-boot:run"]
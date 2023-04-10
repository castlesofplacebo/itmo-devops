FROM eclipse-temurin:17-jdk-jammy as base
WORKDIR /app
COPY .mvn/ .mvn
COPY mvnw pom.xml ./
RUN ./mvnw dependency:resolve
COPY src ./src

FROM base as development
CMD ["./mvnw", "spring-boot:run"]

FROM eclipse-temurin:17-jdk-jammy as production
WORKDIR /app
COPY --from=base /app/target/spring-petclinic-*.jar ./
CMD ["java", "-jar", "/spring-petclinic.jar"]
FROM openjdk
COPY app-code /spring-petclinic
WORKDIR /spring-petclinic
RUN ./mvnw package
FROM openjdk
COPY --from=0 /spring-petclinic/target/spring-petclinic-3.3.0-SNAPSHOT.jar /spring-petclinic/app.jar
WORKDIR /spring-petclinic
CMD ["java", "-jar", "app.jar"]

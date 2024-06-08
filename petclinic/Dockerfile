FROM openjdk
COPY app-code /spring-petclinic
WORKDIR /spring-petclinic
RUN ./mvnw package
CMD ["java", "-jar", "target/spring-petclinic-3.3.0-SNAPSHOT.jar"]

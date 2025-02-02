FROM openjdk:17.0.2-jdk
ARG JAR_FILE=docker/glf-servicediscovery.jar

# Install curl using microdnf
RUN microdnf install -y curl

COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java", "-jar", "/app.jar", "--spring.profiles.active=qa"]
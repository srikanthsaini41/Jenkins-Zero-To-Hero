# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk17:alpine-jre

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# Update the ENTRYPOINT to use Java 17
ENTRYPOINT ["java", "-jar", "app.jar"]

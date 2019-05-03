FROM openjdk:8-jdk-alpine
LABEL maintainer="mihir.chauhan@sftpl.com"
VOLUME /tmp
ARG JAR_FILE=target/gateway-1.0.0-SNAPSHOT.jar
ADD ${JAR_FILE} gateway.jar

# Run the jar file 
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/gateway.jar"]
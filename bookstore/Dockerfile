FROM openjdk:8-jdk-alpine
LABEL maintainer="mihir.chauhan@sftpl.com"
VOLUME /tmp
ARG JAR_FILE=target/bookstore-1.0.0-SNAPSHOT.jar
ADD ${JAR_FILE} bookstore.jar

# Run the jar file 
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/bookstore.jar"]
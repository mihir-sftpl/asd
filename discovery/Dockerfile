FROM openjdk:8-jdk-alpine
LABEL maintainer="mihir.chauhan@sftpl.com"
VOLUME /tmp
EXPOSE 8888
ARG JAR_FILE=target/discovery-1.0.0-SNAPSHOT.jar
ADD ${JAR_FILE} discovery.jar

# Run the jar file 
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/discovery.jar"]
FROM openjdk:8-jdk-alpine
ARG JAR_FILE
COPY application/target/${JAR_FILE} app.jar
COPY file_repo file_repo
EXPOSE 8080
ENTRYPOINT ["java","-Dspring.profiles.active=docker","-jar","/app.jar"]
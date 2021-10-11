FROM openjdk:18-slim-buster
COPY passwordapi.jar /passwordapi.jar
EXPOSE 8080
CMD ["java","--add-opens", "java.base/java.lang=ALL-UNNAMED","-jar","/passwordapi.jar"]

FROM openjdk:8-alpine
EXPOSE 6060
ADD target/demo.jar demo.jar
ENTRYPOINT ["java", "-Dspring.data.mongodb.uri=mongodb://mongod:27017/servers", "-jar", "/demo.jar"]

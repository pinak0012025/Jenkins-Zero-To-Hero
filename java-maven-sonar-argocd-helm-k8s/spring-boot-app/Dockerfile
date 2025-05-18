# Use a maintained and accessible JDK base image
FROM eclipse-temurin:17-jre-alpine

# Define the path to your built JAR file
ARG artifact=target/spring-boot-web.jar

# Set the working directory in the container
WORKDIR /opt/app

# Copy the JAR file into the container
COPY ${artifact} app.jar

# Define the default command to run the JAR
ENTRYPOINT ["java", "-jar", "app.jar"]


# Use a base image with JDK
FROM openjdk:17-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the pom.xml and source code into the container
COPY pom.xml /app
COPY src /app/src

# Install Maven to build the project
RUN apt-get update && apt-get install -y maven

# Build the application using Maven
RUN mvn clean install

# Expose port 8080 (common for Spring Boot apps)
EXPOSE 8080

# Run the application
CMD ["java", "-jar", "target/your-application.jar"]




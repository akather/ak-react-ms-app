# Use an OpenJDK base image - java 17
FROM eclipse-temurin:17-jre-focal

# Add a LABEL to describe what this image is for.
LABEL desc="Image for microservice ms1 in ak-react-ms-app application"

# Set the working directory in the container
WORKDIR /app

# Copy the packaged jar file into the container at the defined working directory
COPY ./target/spring-and-react-0.0.1-SNAPSHOT.jar /app/spring-and-react-0.0.1-SNAPSHOT.jar

# Expose the port that your Spring Boot application uses
EXPOSE 8080

# Define the command to run your application
CMD ["java", "-jar", "spring-and-react-0.0.1-SNAPSHOT.jar"]


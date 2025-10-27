# lockstep-deployment
change
A Spring Boot web application providing a simple "Hello World" REST API.

## Features

- Spring Boot 3.2.0 web application
- RESTful endpoint at `/hello` that returns "Hello World!"
- Comprehensive test coverage with unit and integration tests

## Requirements

- Java 17 or higher
- Maven 3.6 or higher

## Building the Application

```bash
mvn clean package
```

## Running the Application

```bash
mvn spring-boot:run
```

Or run the JAR directly:

```bash
java -jar target/lockstep-deployment-0.0.1-SNAPSHOT.jar
```

The application will start on port 8080.

## Testing the Application

Run all tests:

```bash
mvn test
```

Test the endpoint manually:

```bash
curl http://localhost:8080/hello
```

Expected response: `Hello World!`

## Project Structure

- `src/main/java/com/lockstep/deployment/` - Main application code
  - `LockstepDeploymentApplication.java` - Spring Boot application entry point
  - `HelloController.java` - REST controller with the `/hello` endpoint
- `src/test/java/com/lockstep/deployment/` - Test code
  - `HelloControllerTest.java` - Unit tests for the controller
  - `LockstepDeploymentApplicationTest.java` - Integration tests
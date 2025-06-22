# Eureka-server
A server provided by Spring Cloud to provide user's verification using JWT, registrate microservices and manage their requests to each other
<p align="left">
  <img src="https://skillicons.dev/icons?i=java,spring,gradle,docker,git"/>
</p>

# Features

- 
- 
- 

# Prerequisites
- Java Development Kit(JDK): Version 17 or higher
- Gradle: For project build and dependency management
- Docker: For building container

## Getting Started

Set up Eureka Server locally using Docker Compose for the dev environment.

### Prerequisites

Ensure you have the following installed:
- Java 17
- Gradle
- Docker
  
  ```sh
  java --version
  gradle --version
  docker --version
  ```

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Nightingaale/eureka-server.git
   ```
2. Move to the project directory):
   ```sh
   cd eureka-server
   ```
3. Build microservice with Gradle:
    ```sh
   ./gradlew build
   ```
4. Start the dev environment with Docker Compose:
   ```sh
   docker-compose up -d
   ```
5. Start your microservice:
   ```sh
   ./gradlew bootrun
   ```
6. Verify all services are running:
   ```sh
   docker ps
   ```

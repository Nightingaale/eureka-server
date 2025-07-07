# Eureka-server
A service registry provided by Spring Cloud for microservices architecture
<p align="left">
  <img src="https://skillicons.dev/icons?i=java,spring,gradle,docker,git"/>
</p>

# Features

- Service Registration & Discovery: Allows microservices to dynamically register themselves and discover other services by name, eliminating URLs
- Load Balancing Integration: Enables client-side load balancing (Spring Cloud LoadBalancer) by distributing requests across available service instances
- REST API: Provides access to the service registry, allowing custom integrations and automation

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
2. Move to the project directory:
   ```sh
   cd eureka-server
   ```
3. Build microservice with Gradle:
    ```sh
   ./gradlew build
   ```
4. Start the dev environment with Docker Compose:
   ```sh
   ./gradlew bootrun
   ```
5. Enter Eureka:
   - Access the Eureka UI Server at `http://localhost:8761`
   - (WARNING!) This request `http://localhost:8761/eureka/` is Eureka API, not Eureka Server
  
6. (Optionally):
   - You may use Docker Compose for looking how application actually work in both Spring Boot Container & Docker Container
   - Add dependency in build.gradle `runtimeOnly 'org.springframework.boot:spring-boot-docker-compose'`
   - `docker compose up -d`
   - `8761` - application from Spring Boot Container, `8762` - application from Docker Container

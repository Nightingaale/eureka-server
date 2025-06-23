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
7. Configure Eureka:
   - Access the Keycloak admin console at `http://localhost:8761`
   - (WARNING!) This request `http://localhost:8761/eureka/` is Eureka API, not Eureka Server. You may check this request in Postman

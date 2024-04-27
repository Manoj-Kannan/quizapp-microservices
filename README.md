**Microservices Integration - README**

## Overview

This repository contains the integration of four microservices: `question-service`, `service-registry`, `quiz-service`, and `api-gateway`. Each microservice serves a specific purpose within the system architecture, collectively forming a distributed application.

## Microservices and Ports

1. **question-service**
   - Port: 8080, 8081 (for load balancing)
   - Description: Handles operations related to questions in the system.

2. **service-registry**
   - Port: 8761
   - Description: Eureka server for service discovery and registration.

3. **quiz-service**
   - Port: 8090
   - Description: Manages quizzes and related functionalities.

4. **api-gateway**
   - Port: 8765
   - Description: Acts as an entry point to the system, routing requests to appropriate microservices.

## Setup

1. **Clone Repositories:**
   - Clone the following repositories:
     - [question-service](https://github.com/Manoj-Kannan/question-service.git)
     - [service-registry](https://github.com/Manoj-Kannan/service-registry.git)
     - [quiz-service](https://github.com/Manoj-Kannan/quiz-service.git)
     - [api-gateway](https://github.com/Manoj-Kannan/api-gateway.git)

2. **Build and Run Microservices:**

3. **Configure Ports:**
   - Ensure that each microservice is configured to run on the specified ports as mentioned above.
     
4. **Service Discovery:**
   - `service-registry` acts as a Eureka server for service discovery. Ensure that other microservices register themselves with `service-registry`.
     
5. **Testing Load Balancing:**
   - For `question-service`, you can test load balancing by accessing it on ports 8080 and 8081 simultaneously.

6. **API Gateway Configuration:**
   - Configure `api-gateway` to route requests to appropriate microservices based on their endpoints.

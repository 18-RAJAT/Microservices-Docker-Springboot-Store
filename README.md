# Spring Boot Microservices Bookstore Project

A comprehensive, project-based learning experience in building a microservices-based bookstore application using Spring Boot, Spring Cloud, Docker, and more.

## Overview

This project demonstrates the practical implementation of microservices architecture, creating a fully functional bookstore with various services working together seamlessly.

### Objective

- Build a microservices-based bookstore application using modern tools and frameworks.
- Learn key microservices concepts like asynchronous messaging, resilience, and observability.

## Architecture
<p  align="center">
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">             
<p>

![Image](https://github.com/user-attachments/assets/2cc4a081-b368-472b-b83a-0798b0dc5dd2)


<p  align="center">
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">             
<p>
### Core Microservices

1. **Catalog Service**
   - Manages books in the catalog.
   - Technologies: Spring Boot, Spring Data JPA, PostgreSQL.

2. **Order Service**
   - Manages customer orders.
   - Communication:
     - Synchronous with Catalog Service (via REST).
     - Asynchronous messaging with RabbitMQ.

3. **Notification Service**
   - Sends email notifications.
   - Listens to RabbitMQ event messages.

4. **API Gateway**
   - Routes requests to internal microservices.
   - Aggregates API documentation using Swagger.

## Security and Communication

- **Authentication**: OAuth2 and Keycloak.
- **Communication**:
  - Synchronous: REST API.
  - Asynchronous: RabbitMQ (Message Broker).

## Technology Stack

- **Backend**: Spring Boot 3.x, Java 21.
- **Frontend**: Thymeleaf, Alpine.js, Bootstrap.
- **Development Tools**:
  - Docker, Postman (or alternatives).

## Advanced Features

- **Database Migrations**: Flyway.
- **Resilience**:
  - Circuit breakers, retries, and timeouts with Resilience4j.
- **Distributed Job Locking**: ShedLock to prevent duplicate task execution.

## Monitoring and Observability

- **Monitoring Tools**:
  - Grafana: Visual dashboards.
  - Prometheus: Metrics collection and alerting.
  - Loki: Centralized logging.
  - Tempo: Distributed tracing.

## Development and Testing

- **Testing Frameworks**:
  - JUnit 5, Rest Assured, WireMock for mocking.
- **Local Development**:
  - Docker Compose for streamlined development and testing.

## Deployment

- **Platform**: Docker Compose.
- **Features**:
  - Load balancing using Docker networking.
  - Avoid reliance on Spring Cloud modules like Eureka Server.

## Learning Objectives

- Build scalable and resilient REST APIs.
- Secure microservices with OAuth2 and Keycloak.
- Implement asynchronous messaging with RabbitMQ.
- Utilize advanced deployment and monitoring techniques.

## Recommendations

- Follow along step-by-step to gain hands-on experience.
- Debug and troubleshoot common issues for deeper learning.
- Explore advanced topics like Docker deployment and observability.

# Discovery Server — FinTech Platform

## Overview
The **Discovery Server** is a Netflix Eureka service registry. All microservices in the FinTech platform register themselves with this server on startup. It allows the API Gateway and other services to discover instances dynamically without hardcoded URLs.

## Features
- Service Registration and Discovery
- Health monitoring of registered instances
- Load balancing support via client-side discovery

## Tech Stack
- Java 21 / Spring Boot 3.4.1
- Spring Cloud Netflix Eureka Server

## Port
`8761`

## Configuration
This service typically does not require external environment variables. Just run it.

```bash
mvn spring-boot:run
```

Access the Eureka dashboard at `http://localhost:8761`.

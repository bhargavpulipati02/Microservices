Spring Boot Microservices Architecture
This project demonstrates a microservices architecture using Spring Boot. It includes configuration management, service discovery, API gateway routing, distributed tracing, and business services.
 📌 Architecture Overview

The architecture consists of the following components:

- **Config Server**: Centralized configuration for all services using Spring Cloud Config.
- **Service Registry (Eureka)**: Netflix OSS-based registry for dynamic service discovery.
- **API Gateway**: Routes external requests to internal microservices using Spring Cloud Gateway.

### 🕵️ Distributed Tracing
- **Zipkin**: Traces requests between services to monitor latency and flow.

---

## 🔗 Service Interactions

1. Services fetch config from **Config Server**.
2. They register with **Eureka Service Registry**.
3. API Gateway routes incoming requests to the correct microservice.
4.  ervices call each other using HTTP via logical service names.
5. **Zipkin** collects tracing data for all inter-service communication.



### Prerequisites
- Java 11+
- Maven
- Docker (optional, for Zipkin)




## 📚 Technologies Used

- Spring Boot
- Spring Cloud Config
- Spring Cloud Netflix Eureka
- Spring Cloud Gateway
- Spring Web
- Zipkin for tracing


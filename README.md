# E-Commerce-Backend
SpringBoot Microservices + React


# 🛒 E-Commerce Backend System – Microservices Architecture

![Build](https://img.shields.io/badge/build-passing-brightgreen)
![Spring Boot](https://img.shields.io/badge/spring--boot-2.7+-green)
![MongoDB](https://img.shields.io/badge/database-MongoDB-blue)
![Kafka](https://img.shields.io/badge/messaging-Kafka-orange)
![License](https://img.shields.io/badge/license-MIT-black)

---

## 📸 System Design Overview

![System Design](./ecommerce-hld.png) <!-- Replace with actual file path or hosted image -->

This system is designed using microservices architecture for scalability, modularity, and fault isolation. Each core business domain is managed by a dedicated Spring Boot service, backed by independent MongoDB databases. Kafka is used for asynchronous communication between critical services like Order, Inventory, and Notification.

---

## 🧱 Tech Stack

- **Backend Framework**: Spring Boot (Java)
- **Databases**: MongoDB, Redis
- **API Gateway**: Spring Cloud Gateway
- **Service Discovery**: Eureka
- **Messaging Queue**: Apache Kafka
- **Security**: JWT, RBAC
- **Containerization**: Docker

---

## 🔧 Microservices

| Service         | Description                             | DB         |
|----------------|-----------------------------------------|------------|
| **Auth**        | User registration, login, JWT issuance | MongoDB    |
| **Product**     | Product listing, CRUD operations       | MongoDB    |
| **Cart**        | Session-based cart logic                | Redis      |
| **Order**       | Order placement, history                | MongoDB    |
| **Inventory**   | Stock deduction post-order              | MongoDB    |
| **Notification**| Sends SMS/Email after events via Kafka | N/A        |

---

## 📂 Project Structure



ecommerce-backend/
├── api-gateway/
├── auth-service/
├── product-service/
├── cart-service/
├── order-service/
├── inventory-service/
├── notification-service/

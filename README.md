# Order & Inventory Management System (Microservices Architecture)

A scalable **Order & Inventory Management System** built using **Spring Boot microservices** with a clean layered architecture. The system manages products, orders, customers, shipments, and inventory using distributed services. It supports REST APIs, service discovery, API gateway routing, centralized configuration, and end‑to‑end testing.

---

## 🚀 Features

### ✅ **Core Functionalities**
- Product, Order, Customer, Shipment & Inventory management
- Efficient CRUD operations using MySQL
- Stock validation, order lifecycle management
- Search and filtering endpoints
- Global exception handling and input validation

### ✅ **Microservice Architecture**
- Independent microservices for:
  - **product**
  - **order**
  - **inventory**
  - **customer**
  - **shipment**
  - **OrderlyUI** (frontend)
- **Gateway Service** for routing
- **Eureka Server** for service discovery
- **Config Server** for centralized configuration

### ✅ **Additional Enhancements**
- JWT-based authentication (optional)
- Dockerized services (optional)
- API testing using Postman
- Clean model‑service‑controller layered design

---

## 🗂️ Folder Structure Explanation

- **product-service** → Product creation, updates, retrieval  
- **order-service** → Order creation, status updates, linking customer & inventory  
- **inventory-service** → Stock tracking, quantity validation  
- **customer-service** → Customer registration & profiles  
- **shipment-service** → Shipment assignment & tracking  
- **gateway-service** → Route and secure external API requests  
- **eureka-server** → Registry for microservice discovery  
- **config-server** → Centralized configuration management  
- **OrderlyUI** → Frontend application  

---

## ⚙️ How to Run the Project

✅ 1. Start Config Server
```bash
mvn spring-boot:run

✅ 2. Start Eureka Server
mvn spring-boot:run

✅ 3. Start Gateway Service
mvn spring-boot:run

✅ 4. Start Each Microservice
mvn spring-boot:run

✅ 5. Start UI (OrderlyUI)
npm install
npm start

***📈 Future Enhancements***
Role-based access control (RBAC)
Real-time inventory alerts
Reporting & analytics dashboard
Kafka-based async events
Email/SMS notification service
Payment integration


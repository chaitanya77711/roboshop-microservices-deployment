#  Roboshop Microservices Deployment (Practice Notes)

##  Project Description

This project represents my hands-on practice of deploying the Roboshop microservices application manually on AWS EC2 instances.

I followed the official Roboshop documentation and deployed each service independently to understand how real-world microservices architecture works in production-like environments.

---

##  Project Overview

- Created multiple EC2 instances (t3.micro)
- Installed and configured each service individually
- Connected services using private IP addresses
- Configured systemd services for auto-start
- Verified service health and port accessibility
- Tested complete end-to-end application flow

---

##  Database & Messaging Layer

### MongoDB

- Launched dedicated EC2 instance
- Installed MongoDB server
- Enabled and started MongoDB service
- Loaded catalogue schema
- Verified database status

### MySQL

- Installed MySQL server
- Secured installation
- Created required database and user
- Loaded shipping schema
- Enabled and started MySQL service

### Redis

- Installed Redis
- Enabled and started Redis service
- Verified Redis is active

### RabbitMQ

- Installed Erlang and RabbitMQ
- Created roboshop user
- Set required permissions
- Enabled and started RabbitMQ service

---

##  Application Services

### Catalogue Service (NodeJS)

- Installed NodeJS
- Downloaded application code
- Installed dependencies using npm
- Configured systemd service
- Enabled and started service
- Verified service on port 8080

### User Service (NodeJS)

- Installed NodeJS
- Downloaded application code
- Installed dependencies
- Configured systemd service
- Connected service to MongoDB
- Enabled and started service

### Cart Service (NodeJS)

- Installed NodeJS
- Downloaded application code
- Installed dependencies
- Configured systemd service
- Connected service to Redis
- Enabled and started service

### Shipping Service (Java + Maven)

- Installed Java and Maven
- Built application using Maven
- Copied JAR file
- Configured systemd service
- Connected service to MySQL
- Enabled and started service

### Payment Service (Python)

- Installed Python dependencies
- Downloaded application code
- Configured systemd service
- Connected service to RabbitMQ
- Enabled and started service

---

##  Frontend

- Installed Nginx
- Configured reverse proxy
- Updated configuration to connect backend services
- Enabled and started Nginx
- Verified application access through browser

---

##  Outcome

This project helped me understand real-time DevOps concepts like service management, networking, dependency handling, and application troubleshooting.

It improved my confidence in manually deploying and managing distributed microservices architecture.

🚀 Roboshop Microservices Deployment (Practice Notes)
📖 Project Description

This project represents my hands-on practice of deploying the Roboshop microservices application manually on AWS EC2 instances.

I followed the official Roboshop documentation and deployed each service independently to understand how real-world microservices architecture works in production-like environments.

📌 Project Overview

Created multiple EC2 instances (t3.micro)

Installed and configured each service individually

Connected services using private IP addresses

Configured systemd services for auto start

Verified service health and port accessibility

Tested complete end-to-end application flow

🗄 Database & Messaging Layer
🔹 MongoDB

Launched dedicated EC2 instance

Installed MongoDB server

Enabled and started MongoDB service

Loaded catalogue schema into database

Verified MongoDB service status

🔹 MySQL

Installed MySQL server

Secured MySQL installation

Created required database and application user

Loaded shipping schema

Enabled and started MySQL service

Verified database connectivity

🔹 Redis

Installed Redis

Enabled and started Redis service

Verified Redis is active and reachable

🔹 RabbitMQ

Installed Erlang (dependency)

Installed RabbitMQ server

Created roboshop user

Set required permissions

Enabled and started RabbitMQ service

Verified message broker status

🧩 Application Services Layer
🔹 Catalogue Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies using npm

Configured systemd service

Enabled and started catalogue service

Verified service on port 8080

🔹 User Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd service

Connected service to MongoDB

Enabled and started user service

Verified service status

🔹 Cart Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd service

Connected service to Redis

Enabled and started cart service

Verified service status

🔹 Shipping Service (Java + Maven)

Installed Java

Installed Maven

Downloaded shipping service code

Built application using Maven

Copied generated JAR file

Configured systemd service

Connected service to MySQL

Enabled and started shipping service

Verified service status

🔹 Payment Service (Python)

Installed Python and pip

Downloaded application code

Installed required Python dependencies

Configured systemd service

Connected service to RabbitMQ

Enabled and started payment service

Verified service status

🌐 Frontend Service (Nginx)

Installed Nginx

Downloaded frontend code

Configured reverse proxy for backend services

Enabled and started Nginx

Verified application access via browser

✅ Outcome

Successfully deployed complete Roboshop application manually

Understood service communication via private networking

Gained practical knowledge of systemd service management

Learned database schema loading and dependency handling

Practiced troubleshooting service failures and connectivity issues

Understood real-time DevOps concepts including service management, networking, dependency handling, and application troubleshooting

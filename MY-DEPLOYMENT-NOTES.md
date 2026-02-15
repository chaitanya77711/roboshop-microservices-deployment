🚀 Roboshop Microservices Deployment (Practice Notes)

This project represents my hands-on practice of deploying the Roboshop microservices application manually on AWS EC2 instances.

I followed the official documentation and deployed each service independently to understand real-world microservices architecture.

📌 Project Overview

Created multiple EC2 instances (t3.micro)

Installed and configured services individually

Connected services using private IP addresses

Configured systemd services for auto start

Verified service health and port accessibility

Tested complete application flow

🗄 Database & Messaging Layer
🔹 MongoDB

Launched EC2 instance

Installed MongoDB

Enabled and started MongoDB service

Loaded catalogue schema

Verified MongoDB status

🔹 MySQL

Installed MySQL server

Secured installation

Created database and user

Loaded required schema

Enabled and started MySQL service

🔹 Redis

Installed Redis

Enabled and started Redis service

Verified Redis is active

🔹 RabbitMQ

Installed Erlang

Installed RabbitMQ

Created roboshop user

Assigned permissions

Enabled and started RabbitMQ service

⚙ Application Layer Services
🔹 Catalogue Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies using npm

Configured systemd service

Enabled and started service

Verified service on port 8080

🔹 User Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd service

Connected service to MongoDB

Enabled and started service

🔹 Cart Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd service

Connected service to Redis

Enabled and started service

🔹 Shipping Service (Java + Maven)

Installed Java and Maven

Built application using Maven

Generated JAR file

Configured systemd service

Connected service to MySQL

Enabled and started shipping service

🔹 Payment Service (Python)

Installed Python

Installed required dependencies

Configured systemd service

Connected service to RabbitMQ

Enabled and started payment service

🌐 Frontend Layer
🔹 Nginx

Installed Nginx

Configured reverse proxy

Updated backend routing configuration

Enabled and started Nginx

Verified application in browser

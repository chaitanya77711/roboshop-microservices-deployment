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

Verified database status

🔹 MySQL

Installed MySQL server

Secured installation

Created database and user

Loaded schema

Enabled and started service

🔹 Redis

Installed Redis

Enabled and started Redis

Verified service is active

🔹 RabbitMQ

Installed Erlang

Installed RabbitMQ

Created roboshop user

Assigned permissions

Enabled and started service

⚙ Application Layer Services
🔹 Catalogue Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies (npm install)

Configured systemd service

Started service (Port 8080 verified)

🔹 User Service (NodeJS)

Installed NodeJS

Downloaded code

Installed dependencies

Configured systemd

Connected to MongoDB

Enabled and started service

🔹 Cart Service (NodeJS)

Installed NodeJS

Downloaded code

Installed dependencies

Configured systemd

Connected to Redis

Enabled and started service

🔹 Shipping Service (Java + Maven)

Installed Java & Maven

Built application using Maven

Generated JAR file

Configured systemd service

Connected to MySQL

Enabled and started service

🔹 Payment Service (Python)

Installed Python

Installed required dependencies

Configured systemd service

Connected to RabbitMQ

Enabled and started service

🌐 Frontend Layer
🔹 Nginx

Installed Nginx

Configured reverse proxy

Updated backend routing configuration

Enabled and started Nginx

Verified application in browser

🎯 Key Learnings

Linux service management using systemctl

Microservices communication via private networking

Dependency handling (DB, Cache, Message Queue)

Reverse proxy configuration using Nginx

Troubleshooting using logs & status checks

Real-world DevOps deployment workflow understanding

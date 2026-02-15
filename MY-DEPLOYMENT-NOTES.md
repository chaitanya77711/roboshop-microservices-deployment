MY ROBOSHOP MICROSERVICES DEPLOYMENT (Notes)

This project is my hands-on practice of deploying the Roboshop microservices application manually on AWS EC2 instances.
I followed the official Roboshop documentation and deployed each service separately to understand how real-world microservices architecture works.

What I Did

Created multiple EC2 instances (t3.micro)

Installed and configured each service one by one

Ensured each service runs independently

Connected services using private IP addresses

Configured systemd services for auto start

Verified service health and port accessibility

MongoDB

Launched EC2 instance

Installed MongoDB

Enabled and started MongoDB service

Loaded catalogue schema into database

Verified MongoDB is running

MySQL

Installed MySQL server

Secured installation

Created required database and user

Loaded schema

Enabled and started MySQL service

Redis

Installed Redis

Enabled and started Redis service

Verified Redis is active

RabbitMQ

Installed Erlang

Installed RabbitMQ

Created roboshop user

Set required permissions

Enabled and started RabbitMQ service

Catalogue Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies using npm

Configured systemd service

Enabled and started catalogue service

Verified service running on port 8080

User Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd service

Connected service to MongoDB

Enabled and started user service

Cart Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd service

Connected service to Redis

Enabled and started cart service

Shipping Service (Java + Maven)

Installed Java and Maven

Built application using Maven

Copied generated JAR file

Configured systemd service

Connected service to MySQL

Enabled and started shipping service

Payment Service (Python)

Installed Python and required packages

Downloaded application code

Installed dependencies using pip

Configured systemd service

Connected service to RabbitMQ

Enabled and started payment service

Frontend (Nginx)

Installed Nginx

Configured reverse proxy

Updated configuration to connect backend services

Enabled and started Nginx

Verified application through browser

What I Learned

Service management using systemctl

Inter-service communication using private IP

Dependency handling (DB, Cache, MQ)

Application troubleshooting

Log monitoring and debugging

Real-time microservices architecture understanding

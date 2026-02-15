My Roboshop Microservices Deployment (Notes)

This project is my hands-on practice of deploying the Roboshop microservices application manually on AWS EC2 instances.

I followed the official Roboshop documentation and deployed each service separately to understand how real-world microservices architecture works.

What I Did

I created multiple EC2 instances (t3.micro) and installed each service one by one.
Each service runs independently and communicates using private IP addresses.

MongoDB

Launched EC2 instance

Installed MongoDB

Enabled and started MongoDB service

Loaded catalogue schema into database

Verified MongoDB is running

MySQL

Installed MySQL server

Secured installation

Created database and user

Loaded required schema

Enabled and started MySQL service

Redis

Installed Redis

Enabled and started Redis service

Verified Redis is active

RabbitMQ

Installed Erlang and RabbitMQ

Created roboshop user

Set permissions

Enabled and started RabbitMQ service

Catalogue Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies using npm

Configured systemd service

Enabled and started catalogue service

Verified service on port 8080

User Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd service

Connected service to MongoDB

Enabled and started service

Cart Service (NodeJS)

Installed NodeJS

Downloaded application code

Installed dependencies

Configured systemd

Connected service to Redis

Enabled and started service

Shipping Service (Java + Maven)

Installed Java and Maven

Built application using Maven

Copied JAR file

Configured systemd service

Connected service to MySQL

Enabled and started shipping service

Payment Service (Python)

Installed Python and pip

Installed required packages

Configured systemd service

Connected service to RabbitMQ

Enabled and started payment service

Frontend (Nginx)

Installed Nginx

Copied frontend static files

Configured reverse proxy

Restarted Nginx

Verified application from browser using Public IP

What I Learned

How microservices communicate using internal networking

How to configure systemd services

How to debug service failures using journalctl

How to connect multiple services using environment variables

Basic production-style manual deployment

This project helped me understand real-time DevOps concepts like service management, networking, dependency handling, and application troubleshooting.

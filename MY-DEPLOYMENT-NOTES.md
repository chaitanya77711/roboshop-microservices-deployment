MY ROBOSHOP MICROSERVICES DEPLOYEMENT(Notes)

This project is my hands-on practice of deploying the Roboshop microservices application manually on AWS EC2 instances.
I followed the official Roboshop documentation and deployed each service separately to understand how real-world microservices architecture works.

WHAT I DID
I created multiple EC2 instances (t3.micro) and installed each service one by one.
Each service runs independently and communicates using private IP addresses.

MONGODB
Launched EC2 instance
Installed MongoDB
Enabled and started MongoDB service
Loaded catalogue schema into database
Verified MongoDB is running

MYSQL
Installed MySQL server
Secured installation
Created database and user
Loaded required schema
Enabled and started MySQL service

REDIS
Installed Redis
Enabled and started Redis service
Verified Redis is active

RABBITMQ
Installed Erlang and RabbitMQ
Created roboshop user
Set permissions
Enabled and started RabbitMQ service

CATALOGUE SERVICE(NODE JS)
Installed NodeJS
Downloaded application code
Installed dependencies using npm
Configured systemd service
Enabled and started catalogue service
Verified service on port 8080

USER SERVICE (NODE JS)
Installed NodeJS
Downloaded application code
Installed dependencies
Configured systemd service
Connected service to MongoDB
Enabled and started service

CART SERVICE(NODE JS)
Installed NodeJS
Downloaded application code
Installed dependencies
Configured systemd 
Connected service to Redis
Enabled and started service

SHPPING SERVICE (JAVA + MEAVEN)
Installed Java and Maven
Built application using Maven
Copied JAR file
Configured systemd service
Connected service to MySQL
Enabled and started shipping service

PAYMENT SERVICE(PYTHON)
Installed Python and pip
Installed required packages
Configured systemd service
Connected service to RabbitMQ
Enabled and started payment service

FRONTEND(NGINX)
Installed Nginx
Copied frontend static files
Configured reverse proxy
Restarted Nginx
Verified application from browser using Public IP

WHAT I LEARNED
How microservices communicate using internal networking
How to configure systemd services
How to debug service failures using journalctl
How to connect multiple services using environment variables
Basic production-style manual deployment

THIS PROJECT HELPED ME UNDERSTAND REAL TIME DEVOPS CONCEPTS LIKESERVICE MANAGEMENT NETWORK DEPENDENCY HANDLING AND APPLICATION TROUBLESHOOTING

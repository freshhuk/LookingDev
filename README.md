# LookingDev

## 📌 Introduction

LookingDev is a microservices-based application developed using the Spring framework. Its main purpose is to manage and get developers from platforms such as GitHub, StackOverflow. Quite basic information is collected, such as the user's name, his profile url, and a list of skills and also contains user management (receiving, deleting, etc.).  The application supports authorization using JWT. The Saga pattern were used for architectural solutions

The system consists of four main microservices:

- LookingDev-API: Serves as the API of the application, providing a user-facing interface for receiving requests.
- LookingDev-GitHub: Contains processing and retrieving users from the Git Hub, collecting publicly available information and storing the data in the Potsgres database.
- LookingDev-StackOverflow: Contains processing and retrieving users from Stack Overflow, collecting publicly available information and storing data in a Mongo database.
- LookingDev-Auth: Soon...

To facilitate communication between the microservices, RabbitMQ is used as the message broker. Each microservice is containerized using Docker for ease of deployment and scalability.

## 🛠 Technologies Used

Main
- Java
- SpringFramework(boot, security, web, data)
  
Database
- PostgreSQL
- MongoDB
  
ORM
- Hibernate, JPA
  
Tests
- JUnit/Mockito
  
Tools
- Maven
- Docker/Docker-compose
- RabbitMQ
- JWT

## 📁 Repositories

LookingDev-API:
- https://github.com/freshhuk/LookingDev-API

LookingDev-GitHub:
- https://github.com/freshhuk/LookingDev-GitHub

LookingDev-StackOverflow:
- https://github.com/freshhuk/LookingDev-StackOverflow

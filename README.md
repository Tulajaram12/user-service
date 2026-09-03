# User Service

User microservice for the E-Commerce application.

## Technology

- Java 21
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Maven
- Docker
- Jenkins
- Kubernetes
- Amazon EKS

## APIs

### Register

POST /api/users/register

Request:

{
    "username": "john",
    "email": "john@gmail.com",
    "password": "password123"
}

### Login

POST /api/users/login

Request:

{
    "username": "john",
    "password": "password123"
}

### Get User

GET /api/users/{id}

### Update User

PUT /api/users/{id}

### Delete User

DELETE /api/users/{id}

## Run Locally

mvn spring-boot:run

Application:

http://localhost:8081

## Docker

Build:

docker build -t user-service:1.0 .

Run:

docker run -p 8081:8081 user-service:1.0

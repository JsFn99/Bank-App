# Bank Web App Project

## Overview

This is a Bank Web Application built using a microservice architecture with Spring Boot and Maven on the backend and Angular on the frontend. The application provides functionalities to manage customer accounts, view account details, and perform banking operations.

## Architecture

### Backend
The backend is developed using Spring Boot with the following components:

- **DTOs (Data Transfer Objects):** These are objects used to transfer data between layers and services.
- **Entities:** These are the domain objects representing the data model.
- **Enums:** These represent the fixed set of constants used throughout the application.
- **Exceptions:** Custom exceptions to handle various error scenarios.
- **Mappers:** Classes that map between DTOs and Entities.
- **Repositories:** Interfaces for CRUD operations on entities.
- **Services:** Business logic for the application.
- **Web:** REST controllers handling HTTP requests and responses.

### Frontend
The frontend is developed using Angular with the following components:

- **Accounts:** Components related to account management.
- **Customer Accounts:** Components for managing customer-specific accounts.
- **Customers:** Components for customer management.
- **Model:** Data models used in the application.
- **Navbar:** Navigation bar component.
- **New Customer:** Component for adding new customers.
- **Services:** Angular services for making HTTP requests to the backend.

## Getting Started

### Prerequisites

- Java 11+
- Maven 3+
- Node.js 12+
- Angular CLI

### Backend Setup

1. **Clone the repository:**
    ```bash
    git clone https://github.com/JsFn99/bank-web-app.git
    cd bank-web-app/backend
    ```

2. **Build the project:**
    ```bash
    mvn clean install
    ```

3. **Run the application:**
    ```bash
    mvn spring-boot:run
    ```

### Frontend Setup

1. **Navigate to the frontend directory:**
    ```bash
    cd bank-web-app/frontend
    ```

2. **Install dependencies:**
    ```bash
    npm install
    ```

3. **Run the application:**
    ```bash
    ng serve
    ```

4. **Open your browser and navigate to:**
    ```
    http://localhost:4200
    ```

## Usage

Once the application is running, you can perform the following operations:

- **Manage Customers:** Add, view, update, and delete customer information.
- **Manage Accounts:** Create, view, update, and delete bank accounts.
- **Customer Accounts:** View and manage accounts specific to a customer.

## Demo

A demo video of the application 

![bank-video](bank-video.gif)

## Project Structure

### Backend
```
backend/
├── src/main/java/com/example/bankapp
│   ├── dtos
│   ├── entities
│   ├── enums
│   ├── exceptions
│   ├── mappers
│   ├── repositories
│   ├── services
│   └── web
├── src/main/resources
│   ├── application.properties
│   └── static
└── pom.xml
```

### Frontend
```
frontend/
├── src/app
│   ├── accounts
│   ├── customer-accounts
│   ├── customers
│   ├── model
│   ├── navbar
│   ├── new-customer
│   └── services
├── src/assets
├── src/environments
├── src/styles.css
└── angular.json
```

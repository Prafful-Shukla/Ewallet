# Ewallet
made for self learning

Ewallet is a modular and scalable digital wallet application built using Spring Boot. It simplifies financial transactions, enhances security, and provides seamless functionality by splitting responsibilities into distinct microservices.

---

## Project Overview

The application is divided into four main services:

### 1. **User Service**
- Manages user registration, authentication, and profile management.
- Secures user data with password encryption using Spring Security.
- Provides REST APIs for user-related operations.

### 2. **Wallet Service**
- Handles wallet creation, balance inquiry, and updates.
- Ensures accurate wallet operations with Hibernate and JPA integration.
- Exposes APIs for wallet-related functionalities.

### 3. **Transaction Service**
- Manages all transaction-related operations, including fund transfers and transaction history.
- Guarantees consistency with event-driven communication using Apache Kafka.
- Facilitates smooth transaction handling between wallets.

### 4. **Notification Service**
- Sends notifications (e.g., email) for transaction updates and important events.
- Leverages Spring Boot Mail Starter for reliable email delivery.

---

## Key Features

- **Microservices Architecture**: Independent services for scalability and maintainability.
- **Event-Driven Communication**: Powered by Apache Kafka for seamless interaction between services.
- **Persistent Storage**: Data is securely stored using MySQL.
- **Optimized Caching**: Redis integration for enhanced performance.
- **RESTful APIs**: Well-defined endpoints for easy frontend integration.

---

## Tech Stack

- **Backend**: Java, Spring Boot (REST APIs, Spring Security, Data JPA)
- **Database**: MySQL
- **Messaging**: Apache Kafka
- **Cache**: Redis
- **Notifications**: Spring Boot Mail Starter
- **Build Tool**: Maven

---

## Getting Started

### Prerequisites
Ensure the following tools are installed on your system:
- Java 8 or later
- Maven
- MySQL Server
- Apache Kafka
- Redis Server

### Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Prafful-Shukla/Ewallet.git
   ```

2. Navigate to the root directory:
   ```bash
   cd Ewallet
   ```

3. Build the project using Maven:
   ```bash
   mvn clean install
   ```

4. Start each microservice by navigating to its directory and running:
   ```bash
   mvn spring-boot:run
   ```

### Running Kafka and Redis

- **Kafka**: Start the Kafka server and create required topics for communication between services.
- **Redis**: Ensure the Redis server is running for caching functionality.

---

## Usage

- Access the User Service for registration and authentication.
- Perform transactions through the Transaction Service APIs.
- Check wallet balance or details via the Wallet Service.
- Receive notifications for every successful transaction through the Notification Service.

---

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests to improve this project.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact
For any questions or support, reach out to **Prafful Shukla** at:
- GitHub: [Prafful-Shukla](https://github.com/Prafful-Shukla)

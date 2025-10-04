# Microservice Chat Application

A scalable, modern chat application built using a microservices architecture. This project demonstrates how to design, build, and deploy a chat platform where different services (like messaging, authentication, user profiles, notifications) are separated for improved scalability, maintainability, and resilience.

## Features

- Real-time messaging between users
- User authentication and registration
- Support for multiple chat rooms/groups
- Scalable microservices architecture
- RESTful APIs for communication
- Persistent message storage
- Dockerized deployment for each service

## Architecture

The application is composed of several independent microservices:

- **User Service**: Manages user registration, authentication, and profiles.
- **Chat Service**: Handles creation of chat rooms and manages message exchanges.
- **Notification Service**: Sends real-time notifications to users.
- **Gateway/API Service**: Routes requests to appropriate microservices and handles authentication.
- **Database**: Persistent storage for users, messages, and rooms.

Each microservice can be scaled independently and communicates over HTTP or messaging queues.

## Technologies Used

- Node.js / Express (API development)
- MongoDB or PostgreSQL (storage)
- Docker & Docker Compose (containerization)
- JWT (authentication)
- WebSockets (real-time messaging)
- Redis (message queue, cache)
- Nginx (API Gateway/Load balancer)

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- Node.js (for local development)

### Running Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/WasiqAli22/microservice-chat-application.git
   cd microservice-chat-application
   ```

2. Build and start all services with Docker Compose:
   ```bash
   docker-compose up --build
   ```

3. Each service will be available on its configured port. The API gateway usually runs on `http://localhost:8080`.

### API Documentation

API endpoints are documented using Swagger (if implemented). Visit `http://localhost:8080/api-docs` after starting the services to view documentation.

## Contributing

Contributions are welcome! Please open issues or submit pull requests.

1. Fork the repository.
2. Create a new feature branch (`git checkout -b feature-name`).
3. Commit your changes.
4. Open a pull request.

## License

This project is licensed under the MIT License.

## Contact

For questions or feedback, open an issue or contact [@WasiqAli22](https://github.com/WasiqAli22).
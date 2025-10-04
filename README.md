# Full-Stack Real-Time Chat Application

## Overview

A simple microservice-based chat application:

- **frontend** – React app providing the web UI and communicating via REST & WebSockets.  
- **backend** – Node.js/Express + Socket.io providing REST APIs and real-time messaging.  
- **mongodb** – Separate microservice storing user data, messages, and profiles with persistent storage.

All services are deployed on **Kubernetes**, with each API horizontally scalable. Docker images are pushed to **Docker Hub**.  

---

## Architecture

- **Frontend:** Handles user interactions, communicates with backend.  
- **Backend:** Handles authentication, message CRUD, and real-time events via Socket.io.  
- **Database:** MongoDB stores persistent chat data.  

## Running the Application

- Access frontend: `http://localhost:8080`  
- Backend API: `http://localhost:5001`  
- MongoDB runs as a separate service with persistent storage.  
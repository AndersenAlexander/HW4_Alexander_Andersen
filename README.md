# 🐳 Dockerized Django Project with PostgreSQL & Nginx

This repository contains the solution for **Topic 4 Homework** of the Docker module. It demonstrates how to containerize a multi-service web application using Docker and Docker Compose.

## 🚀 Project Overview

The project consists of three main services running in isolated Docker containers, orchestrated by Docker Compose. The infrastructure is designed to be robust, utilizing healthchecks and persistent volumes.

### Services:
* **`web` (Django):** The main web application built with Python. It handles the backend logic, installs dependencies from `requirements.txt`, and connects to the database.
* **`db` (PostgreSQL):** The database service used for persistent data storage. It includes a custom healthcheck to ensure the database is fully ready to accept connections before the Django application starts.
* **`nginx` (Nginx):** Acts as a reverse proxy, listening on port 80 and forwarding client requests to the Django application container.

## 🛠️ Technologies Used
* Docker & Docker Compose
* Python (3.9+) & Django
* PostgreSQL 16
* Nginx

## ⚙️ How to Run the Project Locally

### Prerequisites
Make sure you have [Docker](https://docs.docker.com/get-docker/) and Docker Compose installed on your machine.

### Running the application

1. **Clone the repository and switch to the correct branch:**
   ```bash
   git clone <your-repository-url>
   cd <repository-folder>
   git checkout lesson-4

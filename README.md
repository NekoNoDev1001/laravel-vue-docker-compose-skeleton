# 🧱 Project Architecture

This repository contains a skeleton for a project with a decoupled architecture, clearly separating the **backend** and the **frontend**, with the goal of facilitating scalability, maintainability, and independent deployment of each service.

---

## Backend – Authentication Service (Laravel)

* The backend is developed using **Laravel** and runs as an independent service responsible for business logic related to user authentication and authorization.
* The service runs inside a Docker container and has its own `docker-compose.yml` configuration file.

## Frontend – Web Application (Node.js + Vue)

* The frontend is a **Single Page Application (SPA)** developed with **Vue.js** and running on **Node.js**.
* This service is also dockerized and has its own independent `docker-compose.yml`.

## Docker Orchestration

* The project includes a root-level `docker-compose.yml` file that allows all services to be started together, simplifying the development environment and ensuring consistency across environments.
* The `.env` file centralizes the environment variables required for container configuration.

## Architecture Benefits

- Clear separation of responsibilities
- Service-level scalability
- Ease of maintenance
- Reproducible environments with Docker
- Simple integration between backend and frontend

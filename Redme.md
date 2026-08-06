## Project Overview

This project demonstrates a three-tier web application deployed using Docker containers without Docker Compose.

Architecture:

Browser
↓
Nginx Frontend
↓
Flask Backend API
↓
MySQL Database

## Features

- Docker Network
- Docker Volumes
- Environment Variables
- Health Checks
- Restart Policies
- Manual Container Deployment
- Backend API
- MySQL Database
- Nginx Reverse Proxy
## Technologies

- Docker
- Nginx
- Python Flask
- MySQL
- Linux

## Build

docker build -t flask-backend:v1 backend/

docker build -t nginx-frontend:v1 frontend/

## Run

(Include all your docker network, volume, and docker run commands here.)

## Screenshots

(Add screenshots of the application, running containers, and browser output.)

## Author

Shaikh Qamre Alam

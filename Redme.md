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

## docker ps -a
alam@DESKTOP-VK19M09:~/three-tier-app/frontend$ docker ps -a
CONTAINER ID   IMAGE          COMMAND                  CREATED             STATUS             PORTS                                 NAMES
b81cfc669c28   1b824473e7fc   "/docker-entrypoint.…"   About an hour ago   Up About an hour   0.0.0.0:80->80/tcp, [::]:80->80/tcp   frontend
271d43bfc0e8   f86e55a80933   "python app.py"          About an hour ago   Up About an hour   5000/tcp                              backend-api
7de8230403b1   mysql:8.0      "docker-entrypoint.s…"   2 hours ago         Up 2 hours         3306/tcp, 33060/tcp                   mysql-db


alam@DESKTOP-VK19M09:~/three-tier-app/frontend$ docker network ls      -------three-tier-net
NETWORK ID     NAME             DRIVER    SCOPE
e373722443ce   bridge           bridge    local
2f40f0c07933   host             host      local
a2ac1bb3054a   none             null      local
1239e2cd1cf0   three-tier-net   bridge    local

alam@DESKTOP-VK19M09:~/three-tier-app/frontend$ docker volume ls            ---- mysql volume
DRIVER    VOLUME NAME
local     minikube
local     mysql-data
## Screenshots


## Author

Shaikh Qamre Alam




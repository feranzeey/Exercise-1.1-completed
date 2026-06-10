HEAD
# Exercise 1.1 - Multi-Service Docker Environment

## Overview

This project demonstrates a multi-service application using Docker Compose. The application consists of:

* React Frontend
* Flask Backend API
* PostgreSQL Database

All services are containerized and managed using Docker Compose.

## Architecture

React Frontend (Port 3000)

↓

Flask Backend (Port 5000)

↓

PostgreSQL Database (Port 5432)

## Technologies Used

* Docker
* Docker Compose
* React
* Flask
* PostgreSQL

## Project Structure

```
Exercise 1.1
├── backend
│   ├── app.py
│   ├── requirements.txt
│   └── Dockerfile
├── frontend
│   └── Dockerfile
├── docker-compose.yml
└── README.md
```

## Build and Run

Build containers:

```bash
docker compose build
```

Start services:

```bash
docker compose up -d
```

Stop services:

```bash
docker compose down
```

## Service URLs

Frontend:

http://localhost:3000

Backend:

http://localhost:5000

Database:

localhost:5432

## Features Implemented

* Multi-container architecture
* Docker Compose orchestration
* Persistent PostgreSQL storage using volumes
* Backend health checks
* Container networking
* Service isolation

## Troubleshooting

### Backend Not Starting

Rebuild backend image:

```bash
docker compose build --no-cache backend
```

### View Logs

```bash
docker compose logs
```

### Check Running Containers

```bash
docker ps
```
# Exercise-1.1-completed
 778f9baa899c1d11e63fd7522a44ba012e144636

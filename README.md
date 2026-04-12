# Nginx Reverse Proxy with Docker Compose

A real-world DevOps setup where Nginx acts as a reverse proxy to route traffic between multiple Flask applications — all managed with Docker Compose.

## Architecture
Internet
↓
Nginx (port 80)
├── /app1/ → Flask App 1 (port 5001)
└── /app2/ → Flask App 2 (port 5002)

## What This Project Does

- Nginx sits at the front and routes incoming requests to the correct app
- Two Flask apps run in isolated Docker containers
- Docker Compose manages all 3 containers with a single command
- Simulates how real companies host multiple services on one server

## Tech Stack

- Nginx
- Flask (Python)
- Docker & Docker Compose
- Linux

## How to Run

```bash
git clone https://github.com/Chinmay03droid/nginx-reverse-proxy.git
cd nginx-reverse-proxy
docker compose up --build
```

Then visit:
- http://localhost/app1/
- http://localhost/app2/

## Author

Chinmay — Aspiring DevOps Engineer
[GitHub](https://github.com/Chinmay03droid)

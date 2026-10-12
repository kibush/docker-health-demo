# Healthcare Docker Lab

A simple healthcare-themed web page served by Nginx, packaged with
Docker, and managed using Docker Compose.

Training project only. No real patient data.

## Requirements

- Docker with Docker Compose

## Run

```bash
docker compose up -d --build
```

Open http://localhost:18083 in your browser.

Allow a few seconds for startup, then verify:

```bash
curl http://127.0.0.1:18083
```

## Stop and remove containers

```bash
docker compose down
```

## Update the application

Edit index.html, then rebuild and deploy:

```bash
docker compose up -d --build
```

## Skills demonstrated

- Building a custom image with a Dockerfile
- Running an application with Docker Compose
- Mapping a localhost port to the container
- Rebuilding and recreating containers after changes
- Verifying HTTP responses with curl

## Project files

- index.html: Web page
- Dockerfile: Image build instructions
- compose.yaml: Build and runtime configuration

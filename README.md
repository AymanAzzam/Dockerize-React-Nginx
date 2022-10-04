# Dockerize React Nginx

This project to:

1. Dockerize React app on development environment using docker compose

2. Deploy React app on Nginx and Dockerize them using docker compose

## Run Development

1. Install Prerequisites

   1. Docker ([Windows](https://docs.docker.com/desktop/windows/install/) - [Linux](https://docs.docker.com/engine/install/ubuntu/))
   2. [Docker Compose](https://docs.docker.com/compose/install/)

2. Run **docker-compose.yaml**

```bash
docker-compose up
```

3. Visit http://localhost:3000

## Run Production

1. Run **docker-compose-prod.yaml**

```bash
docker-compose -f docker-compose-prod.yaml up -d
```

2. Visit http://host:8080

# React + TypeScript + Vite

## Start a developing server inside a Docker container
docker compose up --build

## Run tests in watch mode inside a Docker container
### Solution 1
docker compose up --build
docker exec -it <container_id> npm run test

### Solution 2:
docker compose up --build

## Start a production server with Nginx inside a Docker container
docker build -t prod-react-app .
docker run prod-react-app

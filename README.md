## FastAPI and Traefik Example

This project shows how to setup a FastAPI service behind a Traefik proxy running in docker containers.

### How to setup the project

1. First, add the network to your docker environment: "docker network create hello_network".
2. Spin up the proxy: in the proxy folder run: "docker compose up --build -d".
3. Spin up the hello container which contains the FastAPI: in root folder, run: "docker compose up --build -d"
4. Go to "localhost:8080/dashboard" to see the traefik interface.
5. Go to "hello.localhost/api" to see the api.

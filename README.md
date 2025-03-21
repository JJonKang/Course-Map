# Coursinator.ai

This project consists of a React frontend and a Flask backend, dockerized for local development. Below are the steps to run the application using Docker.

## Requirements

- Docker: [Install Docker](https://docs.docker.com/get-docker/)
- Docker Compose: [Install Docker Compose](https://docs.docker.com/compose/install/)

## Running the Application

1. Getting frontend set up:

    ```bash
    cd frontend && npm install
    ```

2. Getting backend set up:

    ```bash
    cd backend && pip install -r requirements.txt
    ```

3. Build and start the containers:

    ```bash
    docker-compose up --build
    ```

    This will build and start both the **frontend** and **backend** services as specified in the `docker-compose.yml` file.

    The following ports will be exposed:
    - **Frontend (React)**: `http://localhost:3000`
    - **Backend (Flask)**: `http://localhost:5001`


## Stopping the Application

To stop the running containers, simply run:

```bash
docker-compose down
```

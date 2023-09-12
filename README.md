# MyProject

This project contains a Django web application and a Jupyter Notebook, both set up to run in Docker containers.

## Prerequisites

- **Docker**: Ensure you have [Docker](https://www.docker.com/get-started) installed.
- **Docker Compose**: Ensure you have [Docker Compose](https://docs.docker.com/compose/install/) installed.

## Getting Started

Follow these steps to get the environment up and running:

### 1. Clone the Repository:

```bash
git clone [YOUR_REPOSITORY_URL]
cd [YOUR_REPOSITORY_DIRECTORY]
```

### 2. Build and Start the Docker Containers:

```bash
docker-compose build
docker-compose up
```
### 3. Access the Services:

Django App: Once the containers are up and running, the Django app will be accessible at:

```bash
http://localhost:8000/
```

Jupyter Notebook: The Jupyter notebook can be accessed at:

```bash
    http://localhost:8888/
```

4. Stopping the Services:

To stop the services, simply press CTRL+C in the terminal where docker-compose up is running.

Alternatively, you can run the following command in another terminal:

```bash
docker-compose down
```
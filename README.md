# Asynchronous Processing Mechanism HTTP requests

## Prerequisites

Make sure you have Docker and Docker Compose installed on your system. You can download Docker Desktop for your operating system from the official website: https://www.docker.com/get-started

## Getting Started

1. Clone the repository to your local machine:

```bash
git clone https://github.com/arma73/http_processing.git
cd http_processing
```

2. Create a `.env` file:

Copy the `.env.example` file and update the environment variables with your desired values:

```bash
cp .env.example .env
```

3. Run RabbitMQ using Docker Compose:

```bash
docker-compose up -d
```

This will download the RabbitMQ Docker image and start the container in the background.

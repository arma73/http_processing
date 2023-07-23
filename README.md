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

-------

## **TODO**

Step 1: Set up the project structure

- [ ] Define the directory structure:

```
root/
  ├── services/
  │   ├── m1/
  │   │   ├── src/
  │   │   │   ├── controllers/
  │   │   │   ├── routes/
  │   │   │   └── app.ts
  │   │   ├── package.json
  │   │   └── tsconfig.json
  │   └── m2/
  │       ├── src/
  │       │   ├── workers/
  │       │   └── app.ts
  │       ├── package.json
  │       └── tsconfig.json
  ├── docker-compose.yml
  └── README.md
```

Step 2: Set up Docker Compose

- [X] Dockerizing a RabbitMQ instance using Docker containers.
- [ ] Combining both microservices.
- [ ] Enable services for microservices M1 and M2, as well as for RabbitMQ.
- [ ] Configure appropriate dependencies and ports for each service.

Step 3: Development of the M1 microservice

- [ ] Use Express.js and TypeScript for the M1 microservice.
- [ ] Create routes to handle incoming HTTP requests.
- [ ] Add logging with Winston.
- [ ] Create a Dockerfile for the M1 microservice.

Step 4: Development of the M2 microservice

- [ ] Use TypeScript for the M2 microservice.
- [ ] Create job handlers from RabbitMQ.
- [ ] Add logging with Winston.
- [ ] Create a Dockerfile for the M2 microservice.

Step 5: Integration with bit.dev

- [ ] Break your code into reusable components to easily integrate with bit.dev.

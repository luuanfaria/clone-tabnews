# Project Setup Instructions

This repository contains scripts to facilitate the development and testing process of a project using Docker Compose and npm scripts. Follow the instructions below to set up and run the project.

## Prerequisites

- Docker installed on your machine ([Docker Installation Guide](https://docs.docker.com/get-docker/))
- Node.js and npm installed on your machine ([Node.js Installation Guide](https://nodejs.org/en/download/))

## Getting Started

1. Clone this repository to your local machine.

```bash
git clone git@github.com:luuanfaria/clone-tabnews.git
```

2. Navigate to the project directory.

```bash
cd clone-tabnews
```

3. Install project dependencies.

```bash
npm install
```

## Available Scripts

### 1. Start Development Server

To start the development server and bring up the required services using Docker Compose, run:

```bash
npm run dev
```

This command will start the necessary services defined in the `infra/compose.yaml` file using Docker Compose and then start the development server.

### 2. Stop Services

To stop the running services, run:

```bash
docker-compose stop
```

### 3. Shut Down Services

To stop and remove the services, run:

```bash
docker-compose down
```

### 4. Check Code Style

To check the code style using Prettier, run:

```bash
npm run lint:check
```

### 5. Fix Code Style

To automatically fix code style issues using Prettier, run:

```bash
npm run lint:fix
```

### 6. Run Tests

To run tests using Jest, run:

```bash
npm test
```

### 7. Run Tests in Watch Mode

To run tests in watch mode using Jest, run:

```bash
npm run test:watch
```

## Notes

- Ensure that Docker is installed and running on your machine before starting the development server.
- Make sure to run `docker-compose up` before starting the development server (`npm run dev`).

Follow these instructions to get started with the project. If you encounter any issues, refer to the error messages or feel free to reach out for assistance. Happy coding!

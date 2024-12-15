# Learn Docker with a Simple To-Do App

This project is a **basic Node.js application** designed to help you understand how to use Docker and create a `Dockerfile`. The app is a simple to-do list application, but its primary purpose is to serve as a hands-on learning experience for working with Docker containers.

## Features
- A minimal Node.js application.
- Dockerized setup using a `Dockerfile`.
- Exposes the app on port `3000`.

## Prerequisites
Make sure you have the following installed on your system:
- [Node.js](https://nodejs.org/)
- [Docker](https://www.docker.com/)

## How to Use
### 1. Clone the Repository
```bash
git clone https://github.com/sushanth-shetty11/todo-for-learning-docker.git
cd todo-for-learning-docker
```

### 2. Build the Docker Image
Run the following command to build the Docker image:
```bash
docker build -t mytodoapp .
```

### 3. Run the Docker Container
Start a container from the image:
```bash
docker run -it -d -p 3000:3000 mytodoapp
```
The application will be accessible at `http://localhost:3000`.

### 4. Stop the Container
To stop the container, first find the container ID:
```bash
docker ps
```
Then stop it:
```bash
docker stop <container-id>
```

## Project Structure
```
.
├── Dockerfile         # Dockerfile to create the container image
├── package.json       # Node.js project dependencies
├── app.js             # Main application code
└── README.md          # Project documentation
```

## Learning Objectives
- Understand the structure of a `Dockerfile`.
- Learn how to build and run a Docker image.
- Get hands-on experience with Docker commands.

## Key Docker Commands Used
- `docker build`: Build a Docker image from a `Dockerfile`.
- `docker run`: Create and start a container from an image.
- `docker ps`: List running containers.
- `docker stop`: Stop a running container.

## Notes
This project is purely for educational purposes and does not focus on production-level optimizations. It is designed to help beginners familiarize themselves with Docker.

## Contributing
Feel free to submit issues or pull requests to improve this learning resource.

## License
This project is open-source and available under the [MIT License](LICENSE).


## Quick Start Guide for Production

This section provides practical guide for setting up and running the TaciaDocs application for production. The recommended way to get started is by using the provided Docker setup, which orchestrates the frontend and a selected backend automatically.

### Prerequisites

- Git
- Docker and Docker Compose

### 1. Create a Project Directory

First, create a main directory to hold all the TaciaDocs projects. This keeps everything organized.

```bash
mkdir tacia-docs-project
cd tacia-docs-project
```

### 2. Clone the Repositories

You need to clone the backend, the frontend, and the docker projects. You can choose either the Java or JavaScript backend.

**Clone the Backend (choose one):**

```bash
# For the Java backend (recommended for production)
git clone https://github.com/vebulos/tacia-docs-backend-java.git backend-java

# OR for the JavaScript backend (recommended for development)
git clone https://github.com/vebulos/tacia-docs-backend-js.git backend-js
```

**Clone the Frontend and Docker projects:**

```bash
# Clone the frontend
git clone https://github.com/vebulos/tacia-docs-frontend.git frontend

# Clone the Docker project
git clone https://github.com/vebulos/tacia-docs-docker.git docker
```

Your directory structure should now look like this:

```
tacia-docs-project/
├── backend/
├── docker/
└── frontend/
```

### 3. Run the Application

Navigate into the `docker` directory and use the `start-app.sh` script to launch the entire stack.

```bash
cd docker
./start-app.sh
```

The script will build the necessary Docker images and start the containers. Once it's finished, the TaciaDocs application will be available at `http://localhost`.

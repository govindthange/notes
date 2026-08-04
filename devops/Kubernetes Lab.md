# Q. How to build & run microservices on kubernetes locally?

Here's what you need to know:

### Step 1. Create a project that is designed for Kubernetes, not standalone Docker.

GoogleCloudPlatform has a sample project [here..](https://github.com/GoogleCloudPlatform/microservices-demo/blob/9a4616e77f0f9cbcbecaf27d711c38890dda1404/docs/development-guide.md)

The microservices-demo is specifically designed to be flexible:

- Docker-first design: The repository contains Dockerfiles (4.6% of the codebase) for containerizing each of the 10 microservices. This means each service can be built and run independently in containers.

- Kubernetes-agnostic: While the repo is showcasing Kubernetes, the microservices themselves don't require Kubernetes to run. You can:

  1. Build Docker images locally for each microservice
  2. Run them with docker run or docker-compose
  3. Test locally without any cloud infrastructure

- Multi-language support: The services are written in Go (28.9%), Python (27.9%), C# (8.1%), and other languages. Each has its own Dockerfile for containerization.

- No cloud dependencies: The core application logic doesn't inherently depend on cloud-specific services. It's designed to showcase microservices patterns that work anywhere.

To get started locally:

1. Clone the repository
2. Look for a docker-compose.yml file or individual Dockerfiles
3. Build the images: docker build -t service-name .
4. Run with Docker Compose: docker-compose up

2. Then you'll need a local Kubernetes cluster (Minikube or Kind) running on Docker to deploy all microservices together. Here you have two paths:

### Option 1: **Minikube** (Recommended for Linux/Pop!_OS)
```bash
# Prerequisites
minikube start --cpus=4 --memory 4096 --disk-size 32g

# Build and deploy all microservices
skaffold run

# Access the frontend
kubectl port-forward deployment/frontend 8080:8080
# Visit: http://localhost:8080
```

**Requirements:**
- Docker
- kubectl
- Minikube
- Skaffold 2.0.2+
- 4 CPUs, 4GB RAM, 32GB disk

### Option 2: **Kind** (Kubernetes in Docker)
```bash
kind create cluster
skaffold run
```

## Why Not Docker Compose?

This project doesn't include a docker-compose.yml because:
- The 11 microservices communicate via **gRPC**, requiring service discovery
- Each service has complex inter-dependencies
- Kubernetes handles networking, service mesh features (Istio), and orchestration better than Docker Compose

## Build Details

The individual services are containerized (Dockerfiles exist for each), but the application is architected to run as a distributed system on Kubernetes. The main languages are:
- **Go** (28.9%) - frontend, checkout, product catalog, shipping
- **Python** (27.9%) - email, recommendations, load generator
- **Node.js** - currency, payment services
- **Java** - ad service
- **C#** - cart service (Redis-backed)

## What You'll Need

1. **Install Minikube** on Pop!_OS:
   ```bash
   curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-amd64
   sudo install minikube-linux-amd64 /usr/local/bin/minikube
   ```

2. **Install Skaffold**:
   ```bash
   curl -Lo skaffold https://storage.googleapis.com/skaffold/releases/latest/skaffold-linux-amd64
   sudo install skaffold /usr/local/bin/
   ```

3. **Clone and run**:
   ```bash
   git clone https://github.com/GoogleCloudPlatform/microservices-demo
   cd microservices-demo/
   skaffold run
   ```

The first run takes ~20 minutes to build all 11 container images, but it's a fully local, offline experience once complete.

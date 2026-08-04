# Q. How to use Skaffold?

Skaffold has a single command that compiles and builds Docker images for all microservices.

```bash
skaffold build --file-output=build.json
```

This command will:
- **Compile** all 11 microservices (Go, Python, Node.js, Java, C#)
- **Build Docker images** for each service
- **Tag them** with git commit hashes (configurable)
- **Output build metadata** to `build.json` for reference

### If you also want to deploy to Kubernetes immediately:

```bash
skaffold run
```

This does the same build **plus** deploys everything to your local Kubernetes cluster (Minikube/Kind).

# Q. How Skaffold Works?

The [`skaffold.yaml`](https://github.com/GoogleCloudPlatform/microservices-demo/blob/9a4616e77f0f9cbcbecaf27d711c38890dda1404/skaffold.yaml) file lists all 11 microservices and tells Skaffold how to build each one:

```yaml
artifacts:
  - image: emailservice
    context: src/emailservice
  - image: productcatalogservice
    context: src/productcatalogservice
  - image: checkoutservice
    context: src/checkoutservice
  # ... and 8 more services
```

For each service, Skaffold automatically finds the Dockerfile and builds it using Docker.

## Step-by-Step for Pop!_OS

1. **Install Skaffold** (if not already done):
   ```bash
   curl -Lo skaffold https://storage.googleapis.com/skaffold/releases/latest/skaffold-linux-amd64
   sudo install skaffold /usr/local/bin/
   ```

2. **Clone and navigate to the repo**:
   ```bash
   git clone https://github.com/GoogleCloudPlatform/microservices-demo
   cd microservices-demo/
   ```

3. **Just build the images** (no deployment):
   ```bash
   skaffold build
   ```

   Or with a specific registry (e.g., Docker Hub or local registry):
   ```bash
   skaffold build --default-repo=localhost:5000
   ```

4. **View the built images**:
   ```bash
   docker images | grep -E "emailservice|checkoutservice|frontend|etc"
   ```

That's it! All 11 microservices will be compiled and containerized in one command.

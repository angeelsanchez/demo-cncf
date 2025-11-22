# ${{ values.name }}

Landing page for **${{ values.eventTitle }}**

## Architecture

This application is deployed using a GitOps pipeline:

1. **Backstage Scaffolder** creates the repository
2. **GitHub Actions** builds and pushes the container image to Quay.io
3. **ArgoCD** deploys the application to Kubernetes

## Tech Stack

- **Frontend**: Static HTML with CSS animations
- **Container**: Nginx Alpine
- **Registry**: Quay.io
- **Orchestration**: Kubernetes
- **GitOps**: ArgoCD
- **IDP**: Backstage

## Endpoints

| Endpoint | Description |
|----------|-------------|
| `/` | Main landing page |
| `/health` | Health check endpoint |

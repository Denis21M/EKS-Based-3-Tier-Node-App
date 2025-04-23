## 3-Tier .NET Core Application on Amazon EKS

This project showcases the deployment of a 3-tier application—comprised of a .NET 7 Web API, a static UI hosted via Nginx, and a PostgreSQL database—on Amazon EKS using Kubernetes manifests. It demonstrates containerization, Kubernetes deployments and services, persistent storage provisioning, and exposing applications to the internet using an Ingress resource.

## verview

![Architecture](./architecture/project1.jpeg)

The architecture includes:

- Backend: A .NET 7 Web API (Basic3TierAPI) that interfaces with a PostgreSQL database.

- Frontend: A static HTML/CSS/JavaScript UI (Basic3TierUI) served using Nginx.

- Database: A PostgreSQL instance using persistent volume claims for data storage.

Each service is containerized and hosted on Docker Hub. The application is fully deployed on a Kubernetes cluster running in Amazon EKS and accessible externally through an Ingress controller.

## Highlights

- Dockerized backend and frontend services with images pushed to Docker Hub.

- Kubernetes manifests for deployments, services, and persistent volume claims.

- Integration of PostgreSQL using the official container image and persistent storage.

- Application routing via Ingress, making the frontend accessible publicly.

- Scalable, cloud-native architecture leveraging AWS EKS.
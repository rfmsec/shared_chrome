# Containerized shared chrome instance allowing to make a 'joint' purchase, accssible via a novnc webui :)

Repo contains:
1. Dockerfile - Basing on alpine to minimize the size, running chromium browser, fluxbox windowmanager, novnc connected to x11vnc and all supervised by 'supervisor'
2. deploy.yml - K8S Deployment file, Creates a dedicated namespace, deployment, and a Service to expose port 8080 via a LB to allow access to the container.

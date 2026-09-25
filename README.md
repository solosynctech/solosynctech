# SoloSyncTech Website

Company homepage for SoloSyncTech. React + Vite + nginx, containerized for portable deployment.

## Local

    npm install
    npm run dev

## Docker

    docker build -t solosynctech-home .
    docker run --rm -p 8080:80 solosynctech-home

Open http://localhost:8080. Health endpoint: /health.

## Production

Use the same image on Azure Container Apps, GCP Cloud Run, or OCI Container Instances. See docs/architecture.md and the organization infra repository.
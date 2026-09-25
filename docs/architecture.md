# Architecture

Static React/Vite site compiled into an immutable Docker image and served by nginx. No runtime secrets are required.

```mermaid
graph LR
 Browser --> DNS --> Homepage[nginx container]
 Browser --> App[app.solosync.live]
```

Deploy the same image to Azure Container Apps, GCP Cloud Run, or OCI Container Instances. Cloud-specific provisioning belongs in solosynctech/infra.
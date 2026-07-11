# Task 2 - Secure CI/CD Pipeline

## Objective

Build a secure software delivery pipeline that automatically validates code before deployment.

## Pipeline

GitHub Actions performs the following stages:

- Docker Image Build
- Trivy Filesystem Scan
- Trivy Image Scan
- Semgrep Static Analysis
- Gitleaks Secret Detection
- Push Image to GitHub Container Registry (GHCR)

## Security Gates

| Tool | Purpose | Fail Policy |
|-------|----------|------------|
| Trivy | Vulnerability Scan | Fail on Critical findings |
| Semgrep | Static Analysis | Fail on High severity |
| Gitleaks | Secret Detection | Block hardcoded secrets |

## GitOps

Deployment is managed using ArgoCD.

Git becomes the single source of truth.

Automatic synchronization and self-healing are enabled.
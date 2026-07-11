# Architecture

```
                         GitHub Repository
                               │
                               │
                     GitHub Actions CI/CD
                               │
      ┌────────────────────────┼────────────────────────┐
      │                        │                        │
      │                        │                        │
   Semgrep                  Trivy                 Gitleaks
      │                        │                        │
      └────────────── Security Gates ───────────────────┘
                               │
                               ▼
                    Docker Image Build
                               │
                               ▼
                 GitHub Container Registry
                               │
                               ▼
                          ArgoCD GitOps
                               │
                               ▼
                    Kubernetes Cluster
          ┌────────────────────────────────────┐
          │ Namespace: payments                │
          │                                    │
          │ ledger-api Deployment              │
          │ audit-service Deployment           │
          │                                    │
          │ ConfigMap                          │
          │ Secret                             │
          │ ServiceAccount                     │
          │ RBAC                               │
          │ Kyverno Policies                   │
          │ NetworkPolicy                      │
          │ Ingress                            │
          └────────────────────────────────────┘
```

## Security Controls

- Least Privilege RBAC
- Dedicated Service Account
- Non-root Containers
- Read-only Root Filesystem
- RuntimeDefault Seccomp
- Resource Limits
- Health Probes
- GitOps
- Automated Security Scanning
- Admission Control
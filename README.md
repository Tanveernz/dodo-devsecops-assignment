# Dodo Payments – DevSecOps Security Assessment

## Overview

This repository contains my submission for the Dodo Payments Security & DevSecOps Engineer Technical Assessment.

The project focuses on securing a Kubernetes-based payment microservice through workload hardening, secure CI/CD, GitOps, and zero-trust networking principles.

---

## Repository Structure

```
.
├── task1/
│   ├── Kubernetes manifests
│   ├── RBAC
│   ├── Security Context
│   ├── Network Policies
│   └── Kyverno Policies
│
├── task2/
│   ├── GitHub Actions
│   ├── Security Scanning
│   └── Supply Chain Security
│
├── task3/
│   ├── ArgoCD
│   └── Service Mesh
│
├── task4/
│   ├── Recon Report
│   ├── Pentest Report
│   └── Screenshots
│
├── architecture/
└── screenshots/
```

---

# Task Summary

## Task 1 – Workload Hardening

Implemented:

- Kubernetes Deployments
- Services
- ConfigMaps
- Secrets
- Dedicated Service Account
- RBAC
- Security Context
- Read-only Root Filesystem
- Non-root Containers
- RuntimeDefault Seccomp
- Resource Limits
- Health Probes
- Network Policies
- Ingress
- Kyverno Admission Policies

---

## Task 2 – Secure CI/CD

Implemented:

- GitHub Actions
- Docker Image Build
- GitHub Container Registry
- Trivy Filesystem Scan
- Trivy Image Scan
- Semgrep SAST
- Gitleaks Secret Detection
- GitOps using ArgoCD

---

## Task 3 – Zero Trust

Implemented:

- GitOps deployment using ArgoCD
- Automated Sync
- Drift Detection
- Self Heal

Additional work planned:

- Istio mTLS
- Authorization Policies

---

## Task 4 – Security Assessment

Included:

- Reconnaissance Report
- Penetration Test Report
- Risk Analysis
- Remediation Recommendations

---

# Security Decisions

Instead of relying on developers remembering security best practices, security controls were enforced through Kubernetes policies and the CI/CD pipeline.

The repository follows a defense-in-depth approach:

- Least Privilege RBAC
- Secure Containers
- Secret Management
- GitOps
- Automated Security Scanning
- Admission Policies

---

# Technologies

- Kubernetes
- Docker
- GitHub Actions
- ArgoCD
- Kyverno
- Trivy
- Semgrep
- Gitleaks
- GHCR

---

# Screenshots

Screenshots demonstrating deployments, pipeline execution, ArgoCD synchronization, and Kubernetes resources are available inside the `screenshots/` directory.
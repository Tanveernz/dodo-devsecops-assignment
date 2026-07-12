# Dodo Payments – DevSecOps Security Assessment

## Overview

This repository contains my submission for the Dodo Payments Security & DevSecOps Engineer Technical Assessment.

The project focuses on securing a Kubernetes-based payment microservice through workload hardening, secure CI/CD, GitOps, and zero-trust security principles.

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
│   └── GitOps
│
├── task4/
│   ├── README.md
│   ├── reconnaissance.md
│   └── penetration-test-report.md
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
- GitHub Container Registry (GHCR)
- Trivy Filesystem Scan
- Trivy Image Scan
- Semgrep SAST
- Gitleaks Secret Detection
- GitOps using ArgoCD

---

## Task 3 – GitOps

Implemented:

- ArgoCD
- Automated Synchronization
- Drift Detection
- Self Healing

---

## Task 4 – Security Assessment

Included:

- Reconnaissance Report
- Penetration Test Report
- Risk Assessment
- Security Recommendations

---

# Security Decisions

Security was implemented using a defense-in-depth approach.

Implemented controls include:

- Least Privilege RBAC
- Dedicated Service Accounts
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
- GitHub Container Registry (GHCR)

---

# Future Improvements

Given additional time, I would extend this project by implementing:

- Cosign image signing
- SLSA provenance
- Istio service mesh with mTLS
- Sealed Secrets
- Runtime threat detection

---

# Screenshots

Screenshots demonstrating Kubernetes deployments, GitHub Actions, ArgoCD synchronization, RBAC, Kyverno policies, and networking are available in the `screenshots/` directory.
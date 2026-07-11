# Task 1 - Kubernetes Workload Hardening

## Objective

Deploy and secure the ledger-api workload following Kubernetes security best practices.

## Implemented Controls

- Dedicated Namespace
- Deployment
- Service
- Ingress
- ConfigMap
- Secret
- Dedicated ServiceAccount
- Least Privilege RBAC
- Resource Requests & Limits
- Liveness Probe
- Readiness Probe
- Non-root Container
- Read-only Root Filesystem
- RuntimeDefault Seccomp
- Dropped Linux Capabilities
- NetworkPolicy
- Kyverno Admission Policies

## Security Improvements

The original workload contained multiple security weaknesses including hardcoded secrets, root execution, and unrestricted networking.

The deployment was hardened by enforcing least privilege, isolating workloads, implementing Kubernetes admission policies, and separating configuration from application code.

## Verification

The deployment was verified using:

- kubectl
- Kyverno policies
- ArgoCD synchronization
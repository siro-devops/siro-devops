# Siro Collins 
DevOps & Cloud Engineer

> I build cloud infrastructure that's secure, observable, and recovers from failure automatically.

AWS · Azure · Kubernetes · Terraform · CI/CD · Chaos Engineering · GitOps · Security

---

## What I build

| Area | What it looks like in practice |
|---|---|
| **Cloud infrastructure** | Private S3 + CloudFront delivery, VPC networking, EC2 behind ALB, IAM scoped to least privilege — all in Terraform |
| **CI/CD pipelines** | GitHub Actions → Jenkins → Docker → Kubernetes. Commit to production in minutes, automated rollback on failure |
| **GitOps** | ArgoCD watching Git repos automated sync, self-healing, drift correction. No manual kubectl apply |
| **Observability** | Prometheus + Grafana + Loki stacks with SLOs, error budgets, and burn rate alerts |
| **Incident response** | Chaos engineering with LitmusChaos, synthetic monitoring with k6, runbooks for every alert |
| **Security** | Vault secret injection, Trivy CVE scanning, RBAC, network policies, zero hardcoded credentials |

---

## Projects

###  [Kubernetes Incident Response Engineering](https://github.com/siro-devops/k8s-incident-response)
LitmusChaos injects real failures — pod kills, network latency, CPU saturation  while Prometheus fires scoped alerts and k6 synthetic traffic measures user impact in real time. Every failure scenario has a documented runbook mapping detection to recovery.

`LitmusChaos` `Prometheus` `Alertmanager` `k6` `Kubernetes` `Runbooks`

---

###  [GitOps with ArgoCD](https://github.com/siro-devops/argocd-gitops-demo)
Git is the source of truth. ArgoCD watches the repo and automatically syncs the cluster to match no kubectl apply, no manual deployments. Proved automated sync, self-healing, and drift correction.

`ArgoCD` `Kubernetes` `GitOps` `GitHub` `YAML`

---

###  [Multi-environment Terraform with Remote State](https://github.com/siro-devops/multi-env-terraform)
Three isolated environments (dev, staging, prod) deployed from a shared VPC module with S3 remote state and versioning. Each environment has its own CIDR range and state file. No hardcoded values anywhere.

`Terraform` `AWS` `S3` `Modules` `Remote State`

---

###  [Vault Secrets Management on Kubernetes](https://github.com/siro-devops/k8s-vault-secrets)
Zero hardcoded credentials. Vault agent injects secrets at runtime directly into the pod filesystem. No Kubernetes secrets, no environment variables, no credentials in Git. Scoped policy pod can only read one specific path.

`HashiCorp Vault` `Kubernetes` `Helm` `RBAC` `Least Privilege`

---

###  [Container Security Scanning with Trivy](https://github.com/siro-devops/container-security-scanning)
Every Docker image scanned for CVEs before it can deploy. Detected CVE-2026-31789 in python:3.9-slim, pipeline blocked automatically. Upgraded base image, pipeline passed. Shift-left security in practice.

`Trivy` `GitHub Actions` `Docker` `CVE` `Shift-left Security`

---

###  [Kubernetes RBAC and Network Policies](https://github.com/siro-devops/k8s-rbac-network-policies)
Namespace isolation, least-privilege RBAC, and default-deny network policies. Proved yes/no/no with kubectl auth can-i. Blocked cross-namespace traffic then restored selective access with an allow rule.

`Kubernetes` `RBAC` `NetworkPolicy` `Namespace Isolation`

---

###  [SLO Observability Stack](https://github.com/siro-devops/k8s-slo-observability)
99% availability SLO defined, measured, and alerted on in Prometheus. Error budget tracking and multi-window burn rate alerts. Simulated SLO breach and measured error budget consumption in real time.

`Prometheus` `Grafana` `SLOs` `Error Budgets` `Burn Rate Alerts`

---

###  [Kubernetes Autoscaling with HPA](https://github.com/siro-devops/k8s-autoscaling)
Full autoscaling cycle proved end to end. CPU spiked above 50% threshold, HPA scaled from 1 to 3 replicas automatically. Load removed, HPA scaled back to 1 after cooldown.

`Kubernetes` `HPA` `Metrics Server` `Load Testing`

---

###  [Self-hosted GitHub Actions Runners on Kubernetes](https://github.com/siro-devops/k8s-actions-runners)
CI/CD pipeline running inside the Kubernetes cluster using Actions Runner Controller. Runner registered with GitHub, picked up jobs and executed them inside the cluster. No secrets leaving the infrastructure.

`ARC` `GitHub Actions` `Kubernetes` `cert-manager` `Ephemeral Runners`

---

###  [Microservices CI/CD Pipeline](https://github.com/siro-devops/microservices-cicd-pipeline)
Eliminated manual deployments by building an end-to-end pipeline from commit to production in minutes. GitHub Actions triggers the chain Jenkins runs tests, Docker containerises, Kubernetes orchestrates. Zero-downtime with automated rollback.

`Jenkins` `Docker` `Kubernetes` `GitHub Actions`

---

###  [Kubernetes Monitoring Stack](https://github.com/siro-devops/k8s-monitoring-stack)
Full observability platform so nothing breaks silently. Prometheus scrapes metrics, Loki aggregates logs, Grafana surfaces everything in real-time dashboards deployed on Minikube via Helm.

`Kubernetes` `Prometheus` `Grafana` `Loki` `Helm`

---

###  [AWS Terraform Infrastructure](https://github.com/siro-devops/aws-terraform-infrastructure)
Production-grade AWS infrastructure entirely in code. Custom VPC with public and private subnets, EC2 behind ALB, IAM roles scoped to least privilege. Reproducible in any region with a single `terraform apply`.

`Terraform` `AWS` `VPC` `EC2` `ALB` `IAM`

---

###  [Portfolio Dashboard](https://siro-devops.github.io/cicd-demo-app/)
Live site auto-deployed via GitHub Actions on every push. The pipeline itself is the demo.

`GitHub Actions` `GitHub Pages` `CI/CD`

---

## Stack

**Cloud** — AWS (S3, EC2, Lambda, CloudFront, Route 53, IAM, VPC, RDS, CloudWatch, CloudTrail) · Azure (VMs, Blob Storage, AAD, Monitor)

**Containers & orchestration** — Docker · Kubernetes · Helm · Minikube

**IaC & automation** — Terraform · Ansible · GitHub Actions · Jenkins · ArgoCD · ARC

**Security** — HashiCorp Vault · Trivy · RBAC · NetworkPolicy · cert-manager

**Observability** — Prometheus · Grafana · Loki · Alertmanager · k6 · SLOs

**Chaos engineering** — LitmusChaos · Runbooks · Synthetic monitoring

**Languages** — Python · Bash · YAML · HCL

---

## GitHub Stats

![](https://img.shields.io/badge/AWS-Certified-FF9900?style=flat&logo=amazonaws&logoColor=white)
![](https://img.shields.io/badge/Kubernetes-Expert-326CE5?style=flat&logo=kubernetes&logoColor=white)
![](https://img.shields.io/badge/Terraform-IaC-7B42BC?style=flat&logo=terraform&logoColor=white)
![](https://img.shields.io/badge/ArgoCD-GitOps-EF7B4D?style=flat&logo=argo&logoColor=white)
![](https://img.shields.io/badge/Vault-Secrets-000000?style=flat&logo=vault&logoColor=white)
![](https://img.shields.io/badge/Prometheus-Monitoring-E6522C?style=flat&logo=prometheus&logoColor=white)
---

## Available for

Cloud setup and migration · DevOps audits · Infrastructure-as-code builds · Kubernetes deployments · Security hardening · Ongoing cloud operations on AWS and Azure

📧 collins.siro.c@gmail.com ·  [LinkedIn](https://www.linkedin.com/in/siro-collins/) · 🌐 [Portfolio](https://siro-devops.github.io/cicd-demo-app/)

# Siro Collins — DevOps & Cloud Engineer

> I build cloud infrastructure that's secure, observable, and recovers from failure automatically.

AWS · Azure · Kubernetes · Terraform · CI/CD · Chaos Engineering

---

## What I build

| Area | What it looks like in practice |
|---|---|
| **Cloud infrastructure** | Private S3 + CloudFront delivery, VPC networking, EC2 behind ALB, IAM scoped to least privilege — all in Terraform |
| **CI/CD pipelines** | GitHub Actions → Jenkins → Docker → Kubernetes. Commit to production in minutes, automated rollback on failure |
| **Observability** | Prometheus + Grafana + Loki stacks that tell you what's failing, where, and since when — before your users notice |
| **Incident response** | Chaos engineering with LitmusChaos, synthetic monitoring with k6, runbooks for every alert |

---

## Projects

###  [Kubernetes Incident Response Engineering](https://github.com/siro-devops/k8s-incident-response)
The most production-realistic project in this portfolio. LitmusChaos injects real failures — pod kills, network latency, CPU saturation — while Prometheus fires scoped alerts and k6 synthetic traffic measures user impact in real time. Every failure scenario has a documented runbook mapping detection to recovery.

`LitmusChaos` `Prometheus` `Alertmanager` `k6` `Kubernetes` `Runbooks`

---

###  [Microservices CI/CD Pipeline](https://github.com/siro-devops/microservices-cicd-pipeline)
Eliminated manual deployments by building an end-to-end pipeline that takes code from commit to production in minutes. GitHub Actions triggers the chain — Jenkins runs tests, Docker containerises each service, Kubernetes orchestrates the rollout. Zero-downtime deployments with automated rollback on failure.

`Jenkins` `Docker` `Kubernetes` `GitHub Actions`

---

###  [Kubernetes Monitoring Stack](https://github.com/siro-devops/k8s-monitoring-stack)
Full observability platform so nothing breaks silently. Prometheus scrapes metrics, Loki aggregates logs, Grafana surfaces everything in real-time dashboards — deployed on Minikube via Helm. You know what's failing, where, and since when, before your users do.

`Kubernetes` `Prometheus` `Grafana` `Loki` `Helm`

---

###  [AWS Terraform Infrastructure](https://github.com/siro-devops/aws-terraform-infrastructure)
Production-grade AWS infrastructure entirely in code — no clicking through the console. Custom VPC with public and private subnets, EC2 instances behind an Application Load Balancer, IAM roles scoped to least privilege. Reproducible in any region with a single `terraform apply`.

`Terraform` `AWS` `VPC` `EC2` `ALB` `IAM`

---

###  [Portfolio Dashboard](https://siro-devops.github.io/cicd-demo-app/)
Live site auto-deployed via GitHub Actions on every push. The pipeline itself is the demo.

`GitHub Actions` `GitHub Pages` `CI/CD`

---

## Stack

**Cloud** — AWS (S3, EC2, Lambda, CloudFront, Route 53, IAM, VPC, RDS, CloudWatch, CloudTrail) · Azure (VMs, Blob Storage, AAD, Monitor)

**Containers & orchestration** — Docker · Kubernetes · Helm · Minikube

**IaC & automation** — Terraform · Ansible · GitHub Actions · Jenkins

**Observability** — Prometheus · Grafana · Loki · Alertmanager · k6

**Languages** — Python · Bash · YAML · HCL

---

## GitHub Stats

![Siro's GitHub stats](https://github-readme-stats.vercel.app/api?username=siro-devops&show_icons=true&theme=dark&hide_border=true&bg_color=0D1117&title_color=1A56A0&icon_color=FF9900&text_color=8B949E)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=siro-devops&layout=compact&theme=dark&hide_border=true&bg_color=0D1117&title_color=1A56A0&text_color=8B949E)

---

## Available for

Cloud setup and migration · DevOps audits · Infrastructure-as-code builds · Kubernetes deployments · Ongoing cloud operations on AWS and Azure

📧 collins.siro.c@gmail.com ·  [LinkedIn](https://www.linkedin.com/in/siro-collins/) · 🌐 [Portfolio](https://siro-devops.github.io/cicd-demo-app/)

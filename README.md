# 🚀 How to Become a DevOps Engineer in 2026 — Complete Roadmap

> A step-by-step guide from zero to job-ready. Curated by [devops._raj](https://www.instagram.com/devops._raj)

⭐ If this repository helps you, please Star it.
---

## 📌 Table of Contents

- [What is DevOps?](#what-is-devops)
- [Phase 1 — Foundations](#phase-1--foundations-months-1-2)
- [Phase 2 — Version Control & Scripting](#phase-2--version-control--scripting-month-3)
- [Phase 3 — CI/CD](#phase-3--cicd-month-4)
- [Phase 4 — Containers](#phase-4--containers-month-5)
- [Phase 5 — Cloud](#phase-5--cloud-month-6)
- [Phase 6 — Infrastructure as Code](#phase-6--infrastructure-as-code-month-7)
- [Phase 7 — Monitoring & Observability](#phase-7--monitoring--observability-month-8)
- [Phase 8 — Security (DevSecOps)](#phase-8--security-devsecops-month-9)
- [Phase 9 — Advanced & 2026 Trends](#phase-9--advanced--2026-trends-month-10-12)
- [Certifications](#-certifications)
- [Projects to Build](#-projects-to-build)
- [Free Resources](#-free-resources)
- [Timeline Summary](#-timeline-summary)

---

## What is DevOps?

DevOps combines **software development (Dev)** and **IT operations (Ops)** to shorten the software delivery lifecycle. DevOps engineers automate infrastructure, build CI/CD pipelines, manage cloud environments, and ensure systems run reliably at scale.

**In-demand roles in 2026:**
- DevOps Engineer
- Cloud Engineer
- Site Reliability Engineer (SRE)
- Platform Engineer

**Salary range (2026):**
- India: ₹8–35 LPA
- USA: $95,000–$160,000/year

---

## Phase 1 — Foundations (Months 1–2)

### 🐧 Linux & Command Line

Linux is the backbone of DevOps. Every server, container, and cloud VM runs Linux.

**Topics to cover:**
- File system structure (`/etc`, `/var`, `/home`, `/tmp`)
- File permissions (`chmod`, `chown`, `ls -la`)
- Process management (`ps`, `top`, `kill`, `systemctl`)
- Networking basics (`ping`, `curl`, `netstat`, `ss`, `iptables`)
- Shell scripting (loops, conditionals, functions, cron jobs)
- Package management (`apt`, `yum`, `dnf`)
- Text processing (`grep`, `awk`, `sed`, `cut`, `sort`)

**Free resources:**
- 📖 [Linux Journey](https://linuxjourney.com) — beginner-friendly interactive Linux course
- 📖 [The Linux Command Line (free PDF)](https://linuxcommand.org/tlcl.php)
- 🎥 [Linux for Beginners — freeCodeCamp (YouTube)](https://www.youtube.com/watch?v=sWbUDq4S6Y8)
- 🎮 [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) — learn Linux by playing games

---

### 🌐 Networking Basics

**Topics to cover:**
- OSI model and TCP/IP stack
- DNS — how domain resolution works
- HTTP/HTTPS — request/response cycle, status codes
- Load balancing concepts
- Firewalls and security groups
- VPC, subnets, NAT basics (useful for cloud later)

**Free resources:**
- 📖 [Computer Networking: A Top-Down Approach (free chapters)](https://gaia.cs.umass.edu/kurose_ross/online_lectures.htm)
- 🎥 [Networking Fundamentals — Practical Networking (YouTube)](https://www.youtube.com/playlist?list=PLIFyRwBY_4bRLmKfP1KnZA6rZbRHtxmXi)

---

## Phase 2 — Version Control & Scripting (Month 3)

### 🗂️ Git & GitHub

Every DevOps workflow starts with Git.

**Topics to cover:**
- `git init`, `clone`, `add`, `commit`, `push`, `pull`
- Branching strategies (Gitflow, trunk-based development)
- Pull requests and code reviews
- Merge vs rebase
- Git hooks
- GitHub Actions basics (preview — deep dive in Phase 3)

**Free resources:**
- 📖 [Pro Git Book (free)](https://git-scm.com/book/en/v2)
- 🎮 [Learn Git Branching (interactive)](https://learngitbranching.js.org)
- 🎥 [Git and GitHub for Beginners — freeCodeCamp (YouTube)](https://www.youtube.com/watch?v=RGOj5yH7evk)

---

### 🐍 Scripting — Python & Bash

**Topics to cover:**

Bash:
- Shell scripts for automation
- Cron jobs for scheduling
- Error handling in scripts

Python:
- File and directory operations (`os`, `pathlib`)
- HTTP requests (`requests` library)
- Parsing JSON/YAML
- Writing CLI tools with `argparse`
- Boto3 (AWS SDK for Python)

**Free resources:**
- 📖 [Automate the Boring Stuff with Python (free)](https://automatetheboringstuff.com)
- 🎥 [Bash Scripting Tutorial — NetworkChuck (YouTube)](https://www.youtube.com/watch?v=SPwyp2NG-bE)
- 📖 [Python for DevOps (O'Reilly free preview)](https://www.oreilly.com/library/view/python-for-devops/9781492057680/)

---

## Phase 3 — CI/CD (Month 4)

### ⚙️ CI/CD Pipelines

**What to learn:**
- What is CI (Continuous Integration) and CD (Continuous Delivery / Deployment)
- Pipeline stages: Code → Build → Test → Artifact → Deploy
- Writing pipeline-as-code (YAML)

**Tools to learn (pick one to start):**

| Tool | Best for | Free tier |
|------|----------|-----------|
| **GitHub Actions** | GitHub repos, easiest to start | ✅ Yes |
| **GitLab CI** | Self-hosted, full DevOps platform | ✅ Yes |
| **Jenkins** | Most used in enterprise, highly configurable | ✅ Open source |
| **CircleCI** | Fast, easy setup | ✅ Free tier |

> 💡 **Start with GitHub Actions** — it's the easiest to set up and most in-demand in 2026.

**Free resources:**
- 📖 [GitHub Actions official docs](https://docs.github.com/en/actions)
- 🎥 [GitHub Actions Tutorial — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=R8_veQiYBjI)
- 🎥 [Jenkins Full Course — Edureka (YouTube)](https://www.youtube.com/watch?v=7KCS70sCoK0)

---

## Phase 4 — Containers (Month 5)

### 🐳 Docker

**Topics to cover:**
- What is containerization vs virtualisation
- `Dockerfile` — writing and optimising images
- Docker commands: `build`, `run`, `ps`, `exec`, `logs`, `rm`, `rmi`
- Docker volumes and bind mounts
- Docker networking (bridge, host, overlay)
- Docker Compose for multi-container apps
- Image layers and caching
- Publishing images to Docker Hub

**Free resources:**
- 📖 [Docker official docs](https://docs.docker.com/get-started/)
- 🎥 [Docker Tutorial for Beginners — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=3c-iBn73dDE)
- 🎮 [Play with Docker (free browser lab)](https://labs.play-with-docker.com)

---

### ☸️ Kubernetes

**Topics to cover:**
- Architecture: Control plane, worker nodes, etcd, API server
- Core objects: Pod, Deployment, Service, ConfigMap, Secret, Namespace
- `kubectl` commands — the CLI you'll use daily
- Rolling updates and rollbacks
- Horizontal Pod Autoscaler (HPA)
- Ingress and Ingress controllers
- Helm — Kubernetes package manager
- Persistent Volumes (PV) and Persistent Volume Claims (PVC)

**Free resources:**
- 📖 [Kubernetes official docs](https://kubernetes.io/docs/home/)
- 📖 [roadmap.sh/kubernetes](https://roadmap.sh/kubernetes)
- 🎥 [Kubernetes Tutorial for Beginners — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=X48VuDVv0do)
- 🎮 [Killercoda Kubernetes labs (free)](https://killercoda.com/playgrounds/scenario/kubernetes)
- 🎮 [Play with Kubernetes (free browser lab)](https://labs.play-with-k8s.com)

---

## Phase 5 — Cloud (Month 6)

### ☁️ Cloud Platforms

**Pick one to start — AWS is the most in-demand:**

| Platform | Market share | Best cert to start |
|----------|-------------|-------------------|
| **AWS** | ~32% | AWS Cloud Practitioner |
| **Azure** | ~22% | AZ-900 |
| **GCP** | ~12% | Associate Cloud Engineer |

**Core AWS services every DevOps engineer must know:**
- Compute: EC2, ECS, EKS, Lambda
- Storage: S3, EBS, EFS
- Networking: VPC, Route 53, CloudFront, ALB/NLB
- IAM: Users, roles, policies, least privilege
- Database: RDS, DynamoDB, ElastiCache
- Secrets: AWS Secrets Manager, SSM Parameter Store
- Monitoring: CloudWatch, CloudTrail, X-Ray

**Free resources:**
- 📖 [AWS Free Tier](https://aws.amazon.com/free/) — 12 months free on core services
- 🎥 [AWS Full Course — freeCodeCamp (YouTube)](https://www.youtube.com/watch?v=ulprqHHWlng)
- 🎥 [AWS Cloud Practitioner — Andrew Brown (YouTube, free full course)](https://www.youtube.com/watch?v=NhDYbskXRgc)
- 📖 [Cloud Resume Challenge](https://cloudresumechallenge.dev) — build a real project on AWS

---

## Phase 6 — Infrastructure as Code (Month 7)

### 🏗️ Terraform

The #1 IaC tool in 2026. Cloud-agnostic, declarative, and used everywhere.

**Topics to cover:**
- HCL syntax — providers, resources, variables, outputs
- `terraform init`, `plan`, `apply`, `destroy`
- State management and remote state (S3 + DynamoDB for locking)
- Modules — reusable infrastructure components
- Workspaces for environment separation
- Import existing infrastructure

**Free resources:**
- 📖 [Terraform official tutorials](https://developer.hashicorp.com/terraform/tutorials)
- 🎥 [Terraform Tutorial — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=l5k1ai_GBDE)
- 🎮 [Terraform playground on Instruqt (free)](https://developer.hashicorp.com/terraform/tutorials/aws-get-started)

---

### 📦 Ansible

Agentless configuration management. Used to configure servers at scale.

**Topics to cover:**
- Inventory files (static and dynamic)
- Playbooks and roles
- Modules: `apt`, `copy`, `template`, `service`, `docker_container`
- Ansible Vault for secrets
- Idempotency

**Free resources:**
- 📖 [Ansible official docs](https://docs.ansible.com)
- 🎥 [Ansible Full Course — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=1id6ERvfozo)

---

## Phase 7 — Monitoring & Observability (Month 8)

### 📊 The Three Pillars

**Metrics → Prometheus + Grafana**
- Install Prometheus with Node Exporter
- Write PromQL queries
- Build Grafana dashboards
- Set up alerting rules

**Logs → ELK Stack or Loki**
- Elasticsearch + Logstash + Kibana (ELK)
- Or: Grafana Loki + Promtail (lighter, modern)

**Traces → OpenTelemetry + Jaeger**
- Instrument applications with OpenTelemetry
- Visualise request traces across microservices

**Free resources:**
- 📖 [Prometheus official docs](https://prometheus.io/docs/introduction/overview/)
- 🎥 [Prometheus & Grafana Tutorial — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=QoDqxm7ybLc)
- 📖 [Grafana free cloud tier](https://grafana.com/products/cloud/)

---

## Phase 8 — Security (DevSecOps) (Month 9)

Security is now built into the pipeline — not bolted on at the end.

**Topics to cover:**
- Secrets management: HashiCorp Vault, AWS Secrets Manager
- Container image scanning: Trivy, Snyk, Grype
- SAST (Static Application Security Testing): SonarQube, Semgrep
- Dependency scanning: Dependabot, OWASP Dependency-Check
- Supply chain security: Sigstore / cosign for image signing
- IAM least privilege in cloud environments
- Network policies in Kubernetes
- RBAC (Role-Based Access Control)

**Free resources:**
- 📖 [OWASP DevSecOps Guideline (free)](https://owasp.org/www-project-devsecops-guideline/)
- 🎥 [DevSecOps Tutorial — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=aw9bJFuHzcc)
- 📖 [Trivy docs (open source scanner)](https://aquasecurity.github.io/trivy/)

---

## Phase 9 — Advanced & 2026 Trends (Months 10–12)

### 🔥 What's hot in DevOps in 2026

**Platform Engineering**
- Building Internal Developer Platforms (IDPs)
- Tools: Backstage (Spotify), Port, Cortex
- 📖 [platformengineering.org](https://platformengineering.org)

**GitOps**
- Infrastructure and deployments managed via Git
- Tools: ArgoCD, Flux
- 🎥 [ArgoCD Tutorial — TechWorld with Nana (YouTube)](https://www.youtube.com/watch?v=MeU5_k9ssrs)

**AI-assisted DevOps (AIOps)**
- AI-driven anomaly detection and auto-remediation
- Tools: Dynatrace Davis AI, Datadog Watchdog
- GitHub Copilot for writing IaC and pipelines

**eBPF & Advanced Networking**
- Tools: Cilium, Falco (runtime security with eBPF)

**Multi-cloud & Crossplane**
- Managing multiple clouds from one Kubernetes control plane
- 📖 [Crossplane docs](https://crossplane.io)

**Service Mesh**
- Tools: Istio, Linkerd
- mTLS between microservices, traffic management

---

## 🏅 Certifications

Certifications validate your skills and help you get hired faster.

| Certification | Level | Cost | Best for |
|--------------|-------|------|----------|
| [AWS Cloud Practitioner](https://aws.amazon.com/certification/certified-cloud-practitioner/) | Beginner | ~$100 | First cloud cert |
| [AWS Solutions Architect Associate](https://aws.amazon.com/certification/certified-solutions-architect-associate/) | Intermediate | ~$150 | Most in-demand |
| [CKA — Certified Kubernetes Administrator](https://training.linuxfoundation.org/certification/certified-kubernetes-administrator-cka/) | Intermediate | ~$395 | Kubernetes jobs |
| [CKAD — Certified Kubernetes App Developer](https://training.linuxfoundation.org/certification/certified-kubernetes-application-developer-ckad/) | Intermediate | ~$395 | App-focused K8s |
| [HashiCorp Terraform Associate](https://www.hashicorp.com/certification/terraform-associate) | Intermediate | ~$70 | IaC validation |
| [GitHub Actions Certification](https://resources.github.com/learn/certifications/) | Beginner | ~$99 | CI/CD with GitHub |

> 💡 **Recommended order:** AWS CCP → CKA → Terraform Associate

---

## 🛠️ Projects to Build

Real projects matter more than certifications. Build these and put them on GitHub.

| # | Project | Skills demonstrated |
|---|---------|-------------------|
| 1 | **Deploy a web app with Docker + GitHub Actions** | Docker, CI/CD, GitHub Actions |
| 2 | **Deploy app on Kubernetes (local with minikube)** | K8s, kubectl, Helm |
| 3 | **Provision AWS infrastructure with Terraform** | IaC, AWS, remote state |
| 4 | **Set up full monitoring stack (Prometheus + Grafana)** | Observability, alerting |
| 5 | **Build a GitOps pipeline with ArgoCD** | GitOps, ArgoCD, Kubernetes |
| 6 | **Secure a CI/CD pipeline (Trivy + Vault)** | DevSecOps, secrets management |
| 7 | **Cloud Resume Challenge** | AWS, Terraform, CI/CD end-to-end |

---

## 📚 Free Resources

### Best YouTube Channels
- 🎥 [TechWorld with Nana](https://www.youtube.com/@TechWorldwithNana) — best DevOps tutorials
- 🎥 [NetworkChuck](https://www.youtube.com/@NetworkChuck) — Linux, networking, cloud
- 🎥 [That DevOps Guy](https://www.youtube.com/@MarcelDempers) — Kubernetes and GitOps
- 🎥 [Anton Putra](https://www.youtube.com/@AntonPutra) — advanced AWS and Kubernetes
- 🎥 [freeCodeCamp](https://www.youtube.com/@freecodecamp) — full free courses

### Best Free Platforms
- 🌐 [roadmap.sh/devops](https://roadmap.sh/devops) — visual interactive roadmap
- 🌐 [Killercoda](https://killercoda.com) — free browser-based labs for K8s, Linux, Docker
- 🌐 [Play with Docker](https://labs.play-with-docker.com) — free Docker environment
- 🌐 [KodeKloud Engineer](https://kodekloud.com/courses/kodekloud-engineer/) — free hands-on DevOps tasks
- 🌐 [Linux Foundation Free Courses](https://training.linuxfoundation.org/resources/free-courses-a-certifications/) — official Linux courses

### Best Documentation
- 📖 [Kubernetes docs](https://kubernetes.io/docs/)
- 📖 [Terraform docs](https://developer.hashicorp.com/terraform/docs)
- 📖 [Docker docs](https://docs.docker.com)
- 📖 [GitHub Actions docs](https://docs.github.com/en/actions)
- 📖 [AWS docs](https://docs.aws.amazon.com)

---

## ⏱️ Timeline Summary

```
Month 1–2   →  Linux, Networking, OS fundamentals
Month 3     →  Git, Python, Bash scripting
Month 4     →  CI/CD (GitHub Actions + Jenkins)
Month 5     →  Docker → Kubernetes
Month 6     →  Cloud (AWS / Azure / GCP)
Month 7     →  Terraform + Ansible (IaC)
Month 8     →  Prometheus, Grafana, ELK (Observability)
Month 9     →  DevSecOps (Trivy, Vault, SAST)
Month 10–12 →  GitOps, Platform Engineering, AIOps
```

> ⚡ With 2–3 hours/day, you can be job-ready in **6–9 months**. Full-time learners can compress this to **4–6 months**.

---

## 🤝 Follow for Daily DevOps Tips

> 📸 Instagram: [@devops._raj](https://www.instagram.com/devops._raj) — Daily tips, interview Q&A, cheat sheets  
> 💬 Comment **"ROADMAP"** on any post to get free resources in your DM

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=PreethamRaj9121&label=Repo%20Views&color=0e75b6&style=flat" />
</p>

---

*Last updated: June 2026 · Star ⭐ this repo if it helped you*

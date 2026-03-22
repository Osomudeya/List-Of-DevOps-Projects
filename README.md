# DevOps Project Portfolio

I help engineers learn DevOps through **real systems and failures** — not tutorials.

**Production-style labs.**

**A free DevOps learning system.** Pick one:

| | |
| --- | --- |
| **Problem-based lab** | I have a **specific pain** — jump to [Option A](#option-a-problem-based-labs) |
| **Full path** | I want the **whole system** — [Option B](#option-b-become-a-devops-engineer-full-path) |

---

## Most popular labs

| Lab | One line |
| --- | --- |
| **[KubeLab](https://github.com/Osomudeya/kubelab)** | Break Kubernetes safely → understand failures, metrics, and self-healing in real time |
| **[K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab)** | Real secret flows: cloud vault → cluster → pod (ESO, rotation, OIDC) |
| **[DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit)** | Fix real incidents — systematic debugging across the stack |

---

## How this loops

```
  Problem-based lab (narrow pain)
            ↓
  Full path (foundations → core → K8s → cloud → incidents)
            ↓
  Go deeper (labs, guides, repeat under pressure)
            ↓
  Break & debug again ────────────────┘
```

---

## Start here

### Option A: Problem-based labs

*Use this when you have a **specific pain**, not a full curriculum.*

| If your problem is… | Go here |
| --- | --- |
| Kubernetes failures / behavior (drains, OOM, probes, cascading failure, readiness) | [KubeLab](https://github.com/Osomudeya/kubelab) |
| Secrets / vault → cluster → pod (ESO, rotation, env vs volume, EKS/OIDC) | [K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab) |
| Something broke — you need Linux, containers, K8s, cloud, DBs, observability | [DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit) |

*More focused labs (CI/CD, load balancing, etc.) are being added.*

**Need a full system (not a single issue)?** Use **[Option B](#option-b-become-a-devops-engineer-full-path)** (full path).

---

### Option B: Become a DevOps Engineer (full path)

Follow **in order**. Each phase builds on the last.

| Phase | Focus | Repos |
| --- | --- | --- |
| **1 — Foundations** | Local env, containers, GitOps + Cloudflare (edge), end-to-end | [**DevOps Home-Lab 2026**](https://github.com/Osomudeya/DevOps-Home-Lab-2025) |
| **2 — Core DevOps skills** | IaC, CI/CD, K8s, monitoring, multi-environment | [Side DevOps Projects](https://github.com/Osomudeya/side-devops-projects) |
| **3 — Kubernetes & production behavior** | Failure modes, self-heal, observability; secrets & rotation | [KubeLab](https://github.com/Osomudeya/kubelab) → [K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab) |
| **4 — Cloud & infrastructure** | AWS, Jenkins, microservices, enterprise patterns | [AWS DevOps Projects](https://github.com/Osomudeya/Aws-Devops-Projects) |
| **5 — Troubleshooting & real incidents** | Systematic diagnosis across the stack | [DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit) |

After Phase 5, go back to **KubeLab** or **K8s Secrets Lab** to practice under pressure — or use [Gumroad Products (Deep Dive)](#gumroad-products-deep-dive) for structured guides.

---

## The learning path (by phase)

### Phase 1 — Foundations

**You’ll learn:** Compose → k3d → ingress → Prometheus/Grafana → ArgoCD → security → Cloudflare (edge).

**Outcome:** Build → ship → observe → automate → expose globally.

#### [DevOps Home-Lab 2026](https://github.com/Osomudeya/DevOps-Home-Lab-2025)

**Teaches:** Starting from zero, you build a real multi-service app (frontend, API, PostgreSQL, Redis) and take it end-to-end:

- Local development with Docker Compose
- Containerization and Kubernetes (k3d)
- Ingress for stable app routing
- Monitoring with Prometheus and Grafana
- GitOps with ArgoCD (deployments from Git)
- Security basics (network policies, security contexts, secrets)
- Global exposure with Cloudflare (tunnels/CDN, TLS, edge caching)

**Outcome:** You can build, ship, observe, automate, and securely expose a production-style application — from your laptop to a globally reachable, hardened setup.

- **Who should do it:** Beginners to advanced — complete learning path from basics to production

**Next step:** [Side DevOps Projects](https://github.com/Osomudeya/side-devops-projects) — add IaC, CI/CD, and multi-environment patterns.

---

### Phase 2 — Core DevOps skills

**You’ll learn:** Terraform, GitHub Actions, Kubernetes in real pipelines, Prometheus/Grafana, multi-environment infra.

**Outcome:** You can build and operate a standard DevOps toolchain across environments.

#### [Side DevOps Projects](https://github.com/Osomudeya/side-devops-projects)

- **Teaches:** Core DevOps workflows — Infrastructure as Code (Terraform), CI/CD (GitHub Actions), Kubernetes deployments, monitoring (Prometheus/Grafana), and multi-environment infrastructure

- **What’s inside:**
  - Infrastructure provisioning with Terraform (Azure + AWS support)
  - CI/CD pipelines building and deploying containerized apps
  - Kubernetes deployment and scaling
  - Monitoring stack with Prometheus and Grafana
  - Multi-environment setup (dev vs prod using Terraform modules)

- **What you’ll understand:**
  - How DevOps tools connect into a real workflow
  - How to move from local → pipeline → deployment → monitoring
  - How to structure environments like production systems

- **Outcome:** You can build and operate a complete DevOps pipeline across infrastructure, application delivery, and monitoring.

**Next step:** [KubeLab](https://github.com/Osomudeya/kubelab) — see how these systems behave under real failure conditions.

---

### Phase 3 — Kubernetes & production behavior

**You’ll learn:** How clusters fail and recover; probes, limits, state, secrets sync, rotation, cloud-backed patterns.

**Outcome:** You can reason about K8s like production — not just `kubectl apply`.

#### [KubeLab](https://github.com/Osomudeya/kubelab)

- **Teaches:** Kubernetes behavior under real failure conditions — pod crashes, node drains, CPU stress, OOMKills, database issues, cascading failures, readiness probes — with live observability (Prometheus, Grafana, kube-state-metrics)

- **How it works:**
  - Spin up a local cluster (MicroK8s on Multipass or lightweight preview via Docker Compose)
  - Deploy a full stack (React frontend, Node backend, Postgres, monitoring)
  - Trigger failures via UI (or scripts) against a real cluster API
  - Watch metrics and system behavior in real time

- **What you’ll understand:**
  - How Kubernetes self-heals (and where it doesn’t)
  - How failures propagate across services
  - How to read metrics during incidents
  - How this maps to real production debugging and interviews

- **Outcome:** You can reason about Kubernetes like a production system — not just deploy it, but understand how it behaves under pressure.

**Next step:** [K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab) — learn how sensitive data flows securely in real systems.

---

#### [K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab)

- **Teaches:** End-to-end secret management — AWS Secrets Manager → External Secrets Operator (ESO) → Kubernetes → application (env + volume), including IRSA, OIDC, and rotation strategies

- **How it works:**
  - Provision AWS resources with Terraform (Secrets Manager, IAM, optional EKS)
  - Deploy ESO to sync secrets into Kubernetes
  - Run a sample app that consumes secrets via env variables and mounted volumes
  - Observe behavior via UI or app output (validated “match” between env and volume)

- **What you’ll understand:**
  - Secure secret flow without hardcoding in Git
  - IRSA vs static credentials
  - Secret rotation behavior (why volumes update, env doesn’t)
  - ESO vs CSI driver tradeoffs
  - Local (MicroK8s) vs cloud (EKS) setups

- **Outcome:** You can design and implement production-grade secret management across cloud → cluster → application.

**Next step:** [AWS DevOps Projects](https://github.com/Osomudeya/Aws-Devops-Projects) — integrate this into full cloud infrastructure and delivery pipelines.

---

### Phase 4 — Cloud & infrastructure

**You’ll learn:** AWS services, Jenkins, microservices, multi-tier apps, Terraform Cloud patterns.

**Outcome:** You can align your skills with common enterprise AWS + CI/CD setups.

#### [AWS DevOps Projects](https://github.com/Osomudeya/Aws-Devops-Projects)

- **Teaches:** AWS services, Jenkins CI/CD, microservices architecture, multi-tier applications, Terraform Cloud
- **Who should do it:** Intermediate to advanced — AWS-specific implementations and enterprise patterns

**Next step:** [DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit) — systematic diagnosis when the happy path breaks.

---

### Phase 5 — Troubleshooting & real incidents

**You’ll learn:** Methodologies, Linux, containers, K8s, cloud, databases, observability — end to end.

**Outcome:** You can narrow incidents without guessing and explain what you checked.

#### [DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit)

- **Teaches:** End-to-end troubleshooting across the DevOps stack — Linux, containers, Kubernetes, cloud (AWS/Azure/GCP), databases, networking, and observability

- **What’s inside:**
  - Structured troubleshooting guides (Linux → Docker → Kubernetes → Cloud → Databases)
  - Real-world incident scenarios and step-by-step diagnosis
  - Copy-paste commands for fast debugging under pressure
  - Scripts for common workflows (log streaming, event monitoring, repo automation)
  - Observability workflows using Prometheus and Grafana

- **What you’ll understand:**
  - How to approach incidents systematically (not guesswork)
  - How to debug across layers (OS → container → cluster → cloud)
  - How to reduce MTTR using structured thinking and tooling
  - How real production issues map to repeatable troubleshooting patterns

- **Outcome:** You can walk into a broken system, narrow the problem quickly, and explain exactly what you checked and why.

**Next step:** [KubeLab](https://github.com/Osomudeya/kubelab) — simulate failures and practice debugging in a controlled environment.

---

## Gumroad Products (Deep Dive)

Optional resources that go deeper than a typical blog post. This table is designed to help you pick the right one quickly.

| Product | Best for | What you’ll get (high level) | Visual / hands-on (vs just reading) |
| --- | --- | --- | --- |
| **[DevOps Operating System](https://osomudeya.gumroad.com/l/devops-atlas)** *(flagship)* | A single guided path from beginner → hireable | Structured curriculum, build-first progression, capstone portfolio outcomes | Build real infra/projects as you go (not theory-only) |
| **[Complete DevOps Path Bundle v1](https://osomudeya.gumroad.com/l/devops-bundle)** | One cohesive pack covering build → break → fix → explain → automate | A bundle of the core guides + templates in one workflow | Includes hands-on labs + project work across the included resources |
| **[The DevOps Interview Decoder](https://osomudeya.gumroad.com/l/pcpbks)** | Turning “good skills” into interview-ready stories | Decoded interview questions (“what they asked” vs “what they’re testing”), failure-story patterns, prep plan | Practice prompts + project-backed talking points (so you can show, not claim) |
| **[The Kubernetes Detective: Fix It Fast - Complete Troubleshooting Demo](https://osomudeya.gumroad.com/l/jabzk)** | Faster, calmer Kubernetes incident troubleshooting | A step-by-step method, checklists/templates, case studies, practice app, break/fix files | Deploy the sample app and debug intentionally broken scenarios |
| **[Build Your Own DevOps Lab](https://osomudeya.gumroad.com/l/BuildYourOwnDevOpsLab)** | Building a production-style lab on your laptop | Multi-chapter build plan, code/configs, troubleshooting guide, portfolio structure | You build a multi-VM lab + deployable projects (monitoring, CI/CD, k8s) |
| **[AI FOR DEVOPS](https://osomudeya.gumroad.com/l/ai-for-devops)** | Using AI safely for automation + debugging workflows | Tool stack + prompt/workflow system + action plan | Apply workflows to real tasks (debug pods, write scripts, plan systems) |
| **[FREE RESUME TEMPLATE](https://osomudeya.gumroad.com/l/free-resume-template)** | A clean ATS-friendly baseline fast | Resume structure, bullet examples, formatting guidelines, keyword lists | Editable template (you can ship a resume, not just read tips) |
| **[Tip Jar](https://osomudeya.gumroad.com/l/eafkdw)** | Supporting the work | Optional support link | N/A |

**Next step:** Pair any guide with the matching free repo above (e.g. detective content + [KubeLab](https://github.com/Osomudeya/kubelab) / [Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit)).

---

## Medium Articles

- [AWS AND AZURE DevOps Projects Collection](https://medium.com/@osomudeyazudonu/list/devops-projects-419381cab8b1) - All tutorials and guides

---

## Connect

Let's stay connected and learn together!

- **GitHub:** [@Osomudeya](https://github.com/Osomudeya)
- **Medium:** [@osomudeyazudonu](https://medium.com/@osomudeyazudonu)
- **LinkedIn:** [@Osomudeya Zudonu](https://www.linkedin.com/in/osomudeya-zudonu-17290b124/)
- **Twitter:** [@irvingpictures](https://x.com/irvingpictures)

### Questions or Need Help?
- Open an issue in any of the project repositories
- Reach out on social media
- Join the discussion in project comments

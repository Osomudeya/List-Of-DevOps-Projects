# DevOps Project Portfolio

I help engineers learn DevOps through **real systems and failures** — not tutorials. **Everything here is free.** Production-style labs you can run on your laptop today.

**Two ways to use this:** solve **one problem** (first table), or follow the **full path** in order (second table). Details live in each repo’s README.

### By problem

| Problem | Repo |
| --- | --- |
| Kubernetes under stress (drains, OOM, probes, cascading failures, metrics) | [KubeLab](https://github.com/Osomudeya/kubelab) |
| Secrets: cloud → cluster → pod (ESO, rotation, IRSA/OIDC, EKS option) | [K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab) |
| Something broke — Linux, containers, K8s, cloud, DBs, observability | [DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit) |

For a **full system** (not a single issue), use the path below. More narrow labs (e.g. CI/CD-only) are planned.

### Full path (in order)

| Step | Repo | What you build |
| --- | --- | --- |
| 1 | [**DevOps Home-Lab 2026**](https://github.com/Osomudeya/DevOps-Home-Lab-2025) | Multi-service app: Compose, k3d, ingress, Prometheus/Grafana, ArgoCD, security basics, Cloudflare (edge) |
| 2 | [Side DevOps Projects](https://github.com/Osomudeya/side-devops-projects) | Terraform (AWS/Azure), GitHub Actions, K8s deploys, Prometheus/Grafana, multi-env |
| 3 | [KubeLab](https://github.com/Osomudeya/kubelab) then [K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab) | Failure modes + observability; then secret sync, rotation, env vs volume |
| 4 | [AWS DevOps Projects](https://github.com/Osomudeya/Aws-Devops-Projects) | AWS, Jenkins, microservices, Terraform Cloud–style patterns |
| 5 | [DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit) | Systematic incident flow across the stack |

After step 5, loop back to **KubeLab** or **K8s Secrets Lab** under pressure, or use [Gumroad Products (Deep Dive)](#gumroad-products-deep-dive) for guided deep dives.

---

## Project index

**[DevOps Home-Lab 2026](https://github.com/Osomudeya/DevOps-Home-Lab-2025)** — From zero to a globally exposed, hardened stack (Compose → k3d → GitOps → Cloudflare). **Next:** [Side DevOps Projects](https://github.com/Osomudeya/side-devops-projects).

**[Side DevOps Projects](https://github.com/Osomudeya/side-devops-projects)** — IaC, CI/CD, K8s, monitoring, multi-environment as one workflow. **Next:** [KubeLab](https://github.com/Osomudeya/kubelab).

**[KubeLab](https://github.com/Osomudeya/kubelab)** — Break K8s on purpose; watch metrics and self-heal in real time. **Next:** [K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab).

**[K8s Secrets Lab](https://github.com/Osomudeya/k8s-secret-lab)** — AWS Secrets Manager → ESO → workloads (env + volume), rotation, local or EKS. **Next:** [AWS DevOps Projects](https://github.com/Osomudeya/Aws-Devops-Projects).

**[AWS DevOps Projects](https://github.com/Osomudeya/Aws-Devops-Projects)** — Enterprise-style AWS + delivery. **Next:** [DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit).

**[DevOps Troubleshooting Toolkit](https://github.com/Osomudeya/DevOps-Troubleshooting-Toolkit)** — Guides, scenarios, commands, scripts, observability patterns across layers. **Next:** [KubeLab](https://github.com/Osomudeya/kubelab) to rehearse in a safe cluster.

---

## Gumroad Products (Deep Dive)

Optional resources that go deeper than a typical blog post. This table is designed to help you pick the right one quickly.

| Product | What you get |
| --- | --- |
| **[DevOps Operating System](https://osomudeya.gumroad.com/l/devops-atlas)** *(flagship)* | One end-to-end path: local stack through K8s and CI/CD, production-style tickets, and a capstone portfolio project |
| **[Complete DevOps Path Bundle v1](https://osomudeya.gumroad.com/l/devops-bundle)** | Five products together: AI-for-DevOps guide, laptop lab book, K8s troubleshooting system, interview decoder, and resume template |
| **[The DevOps Interview Decoder](https://osomudeya.gumroad.com/l/pcpbks)** | Decoded questions (what they asked vs what they test), failure-story patterns, and a short prep plan |
| **[The Kubernetes Detective: Fix It Fast - Complete Troubleshooting Demo](https://osomudeya.gumroad.com/l/jabzk)** | Troubleshooting method (STOP framework), long-form guide, break/fix assets, sample app, and production-style case studies |
| **[Build Your Own DevOps Lab](https://osomudeya.gumroad.com/l/BuildYourOwnDevOpsLab)** | Six-chapter build: virtualization, Docker/K8s, Terraform/Ansible, monitoring, CI/CD, and a simulated multi-VM “prod” environment |
| **[AI FOR DEVOPS](https://osomudeya.gumroad.com/l/ai-for-devops)** | Coordinated prompts and workflows across major AI tools, plus a concrete multi-week action plan |
| **[FREE RESUME TEMPLATE](https://osomudeya.gumroad.com/l/free-resume-template)** | Full layout, 20+ example bullets you can steal, ATS notes, and keyword guidance |

**Newsletter**

Every week — one real case study, one tactic, one honest moment where something broke. No padding.

[Subscribe](https://osomudeya.gumroad.com/subscribe)

---

## Medium

- [AWS AND AZURE DevOps Projects Collection](https://medium.com/@osomudeyazudonu/list/devops-projects-419381cab8b1)

## Connect

- **GitHub:** [@Osomudeya](https://github.com/Osomudeya)
- **Medium:** [@osomudeyazudonu](https://medium.com/@osomudeyazudonu)
- **LinkedIn:** [@Osomudeya Zudonu](https://www.linkedin.com/in/osomudeya-zudonu-17290b124/)

Questions: open an issue on a project repo or reach out on the channels above.

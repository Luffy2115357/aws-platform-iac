# aws-platform-iac

## 🚀 The Architecture
*(Diagram coming soon!)*
* **Developer Push:** Code is pushed to `core-services-api`.
* **CI Factory:** GitHub Actions tests code, runs security scans, and packages the application.
* **CD Engine:** ArgoCD detects changes in this repository and automatically syncs the live AWS EKS cluster.
* **Observability:** Prometheus and Grafana monitor cluster health.

## 📂 Repository Structure
* `/terraform` - AWS Infrastructure state (VPC, EKS).
* `/kubernetes` - GitOps source of truth (ArgoCD apps, security policies).
* `/helm-charts` - Packaged deployment templates.
* `/docs` - System design and architectural decisions.
* `/screenshots` - Proof of execution.

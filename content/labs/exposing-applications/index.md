# Exposing applications

In this QBR workshop track you follow the same **learning path** as [Exposing applications](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/Exposing_Applications/) in **Cloudera Cloud Factory** documentation: from Kubernetes DNS fundamentals through **LoadBalancer**, **Taikun Ingress**, **Managed Apps**, **CertManager**, and **Taikun Link**.

You will see how workloads running in Kubernetes can reach **users, internal teams, and services outside the cluster** in a secure, repeatable way—whether you need a quick internal dashboard or production HTTPS with automated certificates.

Use each **workshop module** below for facilitator-led steps and checklists; open the linked **official documentation** for full screenshots, API details, and edge cases.

---

## Ways to expose applications

### 01. Kubernetes DNS — basics

- Learn how **DNS** works in Kubernetes and how **Services** are resolved inside and outside the cluster.
- Understand **CoreDNS** and how the cluster assigns DNS names to **Pods** and **Services**.

[Open workshop module 01](01-kubernetes-dns-basics.md){ .md-button } [Full documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/01_Kubernetes_DNS-Basics/)

### 02. LoadBalancer

- Understand **LoadBalancer** `Service` types, when they apply, and how they expose workloads.
- Relate **cloud provider** integration to what you see in Cloud Factory.

[Open workshop module 02](02-loadbalancer.md){ .md-button } [Full documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/02_LoadBalancer/)

### 03. Taikun Ingress — basics

- Introduction to **Taikun Ingress** for HTTP/HTTPS exposure, annotations, and architecture.
- Practice designing **ingress rules** that stay maintainable as applications grow.

[Open workshop module 03](03-taikun-ingress-basics.md){ .md-button } [Full documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/03_Taikun_Ingress-Basics/)

### 04. Taikun Ingress — Managed Apps

- Expose applications installed via **Managed Apps** using Ingress patterns the platform supports.
- See how **pre-configured** exposure reduces manual Ingress YAML for common tools.

[Open workshop module 04](04-taikun-ingress-managed-apps.md){ .md-button } [Full documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/04_Taikun_Ingress-Managed_Apps/)

### 05. Taikun Ingress — CertManager

- Use **CertManager** with Taikun Ingress to **automate TLS** provisioning and renewal.
- Discuss **production** practices for continuous HTTPS.

[Open workshop module 05](05-taikun-ingress-certmanager.md){ .md-button } [Full documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/05_Taikun_Ingress-CertManager/)

### 06. Taikun Link

- **Taikun Link** exposes services with a **dedicated hostname and HTTPS** with minimal DNS/certificate work.
- Walk through activation and a **time-to-access** story suitable for QBR.

[Open workshop module 06](06-taikun-link.md){ .md-button } [Full documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/06_Taikun_link/)

---

## Before this track

Complete [Environment & project access](../environment-setup.md) so you are signed in, inside the correct **project**, and on the agreed **cluster**.

[Start with module 01 — Kubernetes DNS basics](01-kubernetes-dns-basics.md){ .md-button .md-button--primary }

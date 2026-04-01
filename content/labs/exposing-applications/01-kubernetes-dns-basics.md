# 01 · Kubernetes DNS — basics

This module mirrors **[01 Kubernetes DNS-Basics](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/01_Kubernetes_DNS-Basics/)** in the product documentation.

## What you will learn

- How **DNS** resolves **Services** and **Pods** inside the cluster.
- The role of **CoreDNS** and **cluster-internal** names.
- Why **in-cluster** DNS is the foundation before **LoadBalancer** and **Ingress**.

## Workshop exercise (facilitator-led)

1. In your workshop cluster, pick a **Namespace** that contains a running **Deployment** and **Service** (or create a minimal example per facilitator script).
2. From the UI or `kubectl`, show the **Service** name and **ClusterIP** (or headless pattern if your script uses it).
3. Demonstrate **DNS resolution** from inside a pod (for example `nslookup` / `dig` to `<service>.<namespace>.svc.cluster.local`) or the equivalent your environment allows.
4. Contrast **cluster-internal** DNS with **external** names—why users still need **LoadBalancer** or **Ingress** for browser access.

!!! tip "Narration for QBR"
    Emphasize **predictable naming** and **service discovery** as prerequisites for platform governance and multi-team clusters.

## Checklist

- [ ] Audience sees **where** Kubernetes stores DNS configuration (high level).
- [ ] Audience can name **one** reason internal DNS alone is not enough for public apps.

**Full procedure and diagrams:** [Kubernetes DNS basics — documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/01_Kubernetes_DNS-Basics/)

[Next: 02 · LoadBalancer](02-loadbalancer.md){ .md-button .md-button--primary }

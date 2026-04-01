# 03 · Taikun Ingress — basics

This module mirrors **[03 Taikun Ingress-Basics](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/03_Taikun_Ingress-Basics/)** in the product documentation.

## What you will learn

- **Taikun Ingress Controller** role for **HTTP/HTTPS** routing into the cluster.
- **Annotations** and **rules** at a high level (host, path, backend Service).
- How to keep **ingress rules** structured as application count grows.

## Workshop exercise (facilitator-led)

1. Open **Ingress** (or **Routes**) in the Cloud Factory UI for the workshop namespace.
2. Walk through **one** ingress resource: **hostname**, **path**, **backend service:port**.
3. Optional: show **TLS** section at a high level (details in module 05).
4. Relate to **module 01**: how DNS for the **public hostname** points to the **ingress entry point**.

!!! tip "QBR angle"
    Position Ingress as the **standard L7 front door** for many microservices behind **one** entry.

## Checklist

- [ ] Audience sees **host + path → service** mapping in the UI or YAML.
- [ ] Audience understands **Ingress** complements **internal DNS** from module 01.

**Full procedure:** [Taikun Ingress basics — documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/03_Taikun_Ingress-Basics/)

[Previous: 02 · LoadBalancer](02-loadbalancer.md){ .md-button } [Next: 04 · Managed Apps](04-taikun-ingress-managed-apps.md){ .md-button .md-button--primary }

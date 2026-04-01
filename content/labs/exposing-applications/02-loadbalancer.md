# 02 · LoadBalancer

This module mirrors **[02 LoadBalancer](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/02_LoadBalancer/)** in the product documentation.

## What you will learn

- The **LoadBalancer** `Service` type and how the cloud / platform provisions an external endpoint.
- When **LoadBalancer** is appropriate versus **Ingress** (cost, protocols, L4 vs L7).
- **Best practices** for test vs production exposure (facilitator examples).

## Workshop exercise (facilitator-led)

1. Identify a **Service** that can be patched or created as type **LoadBalancer** (or use a UI workflow your tenant supports).
2. Show **pending → external IP / hostname** (or provider-specific status) and open the **endpoint** with a simple HTTP check if allowed.
3. Discuss **security**: firewall rules, who can reach the endpoint, and when **Ingress + TLS** is preferable.

!!! warning "Workshop safety"
    Use **non-production** clusters and **sanitized** sample apps. Do not expose internal service names or credentials on shared screens.

## Checklist

- [ ] Audience sees **one** successful **LoadBalancer** path end-to-end (or a clear simulated step).
- [ ] Audience can compare **LoadBalancer** vs **Ingress** in one sentence.

**Full procedure:** [LoadBalancer — documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/02_LoadBalancer/)

[Previous: 01 · DNS basics](01-kubernetes-dns-basics.md){ .md-button } [Next: 03 · Taikun Ingress basics](03-taikun-ingress-basics.md){ .md-button .md-button--primary }

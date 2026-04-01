# 04 · Taikun Ingress — Managed Apps

This module mirrors **[04 Taikun Ingress-Managed Apps](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/04_Taikun_Ingress-Managed_Apps/)** in the product documentation.

## What you will learn

- How **Managed Apps** (catalog-installed software) integrate with **Ingress** in Cloud Factory.
- **Pre-configured** or guided exposure paths that reduce custom YAML for common tools (monitoring, CI/CD, etc.).
- When **Managed App** ingress patterns save operations time.

## Workshop exercise (facilitator-led)

1. Open **Applications** / **Managed Apps** (or your tenant’s equivalent) and select **one** app the QBR script standardizes on (for example a dashboard or toolchain).
2. Show **exposure** or **access** settings the catalog provides (hostname, ingress toggle, etc.).
3. Validate **HTTPS** or **HTTP** access per script—link forward to **module 05** if certificates are automated via **CertManager**.

!!! example "Customize"
    Swap the sample app for whatever your **Budapest QBR** demo standardizes on; keep the **story**: *catalog → ingress → URL*.

## Checklist

- [ ] Audience sees **Managed App → reachable URL** without writing raw Ingress from scratch (or sees the minimal YAML the UI generates).
- [ ] Audience can name **one** ops benefit (time to value, consistency).

**Full procedure:** [Taikun Ingress — Managed Apps — documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/04_Taikun_Ingress-Managed_Apps/)

[Previous: 03 · Ingress basics](03-taikun-ingress-basics.md){ .md-button } [Next: 05 · CertManager](05-taikun-ingress-certmanager.md){ .md-button .md-button--primary }

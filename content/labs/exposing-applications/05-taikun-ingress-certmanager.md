# 05 · Taikun Ingress — CertManager

This module mirrors **[05 Taikun Ingress-CertManager](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/05_Taikun_Ingress-CertManager/)** in the product documentation.

## What you will learn

- How **CertManager** integrates with **Taikun Ingress** to obtain and **renew TLS certificates**.
- **Production-oriented** practices: issuer types, renewal windows, and failure visibility.
- Relationship between **DNS**, **Ingress hostnames**, and **certificate** SANs.

## Workshop exercise (facilitator-led)

1. Pick an **Ingress** hostname that is allowed for the workshop (sandbox domain or facilitator-provided).
2. Show **TLS secret** or **Certificate** resource state in the UI or `kubectl` (Ready / Issuing).
3. Open **https://** in the browser and inspect **certificate** validity at a high level (issuer, expiry).
4. Briefly mention **renewal**—why automation matters for QBR customer conversations (compliance, uptime).

!!! tip "Executive summary"
    One line: **“Certificates renew without a ticket to the infrastructure team.”**

## Checklist

- [ ] Audience sees **HTTPS** working for at least **one** ingress host (or a clear dry-run).
- [ ] Audience connects **CertManager** to **continuous** TLS, not one-time manual upload.

**Full procedure:** [Taikun Ingress — CertManager — documentation](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/05_Taikun_Ingress-CertManager/)

[Previous: 04 · Managed Apps](04-taikun-ingress-managed-apps.md){ .md-button } [Next: 06 · Taikun Link](06-taikun-link.md){ .md-button .md-button--primary }

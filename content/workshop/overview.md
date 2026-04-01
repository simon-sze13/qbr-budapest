# Cloud Factory overview (QBR narrative)

## Elevator pitch

**Cloudera Cloud Factory** helps enterprises run Kubernetes and application platforms consistently across **public and private clouds**—with guardrails, observability, and deployment patterns that match how regulated and data-heavy organizations operate.

## Why it shows up in QBR

| Theme | Talking point |
|--------|----------------|
| **Multi-cloud reality** | One operational model instead of one-off tooling per cloud. |
| **Time to value** | Standardized clusters, apps, and policies reduce bespoke automation. |
| **Governance** | Projects, roles, and policies align with enterprise security expectations. |
| **Data & AI adjacency** | Fits next to Cloudera data platform stories—same buyer, complementary footprint. |

## Map to the labs (Exposing applications)

Aligned with [Exposing applications](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/Exposing_Applications/) in product documentation:

1. **Environment & project** — Governed project and cluster context before any exposure.
2. **01–02** — **Internal DNS** then **LoadBalancer** as the first external path.
3. **03–05** — **Ingress** stack: basics, **Managed Apps**, **CertManager** for HTTPS.
4. **06 — Taikun Link** — Fast, secure URL without heavy DNS/TLS setup.
5. **Wrap-up** — Talk tracks and [full documentation](https://docs.taikun.cloud/).

!!! tip "Customize this page"
    Replace generic bullets with **named customer outcomes** (for example FinServ, manufacturing, telco) before your QBR dry run.

---
hide:
  - toc
---
# Cloudera Cloud Factory — QBR workshop

Welcome to the **QBR hands-on workshop** for **Cloudera Cloud Factory**.

You will work through **environment access**, then the **Exposing applications** track in the same order as the product documentation: from **Kubernetes DNS** and **LoadBalancer**, through **Taikun Ingress** (including **Managed Apps** and **CertManager**), to **Taikun Link**. Each lab page links to the matching chapter on **[docs.taikun.cloud](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/Exposing_Applications/)** for full detail. Finish with **Workshop wrap-up** for discussion prompts.

---

## Start here

<div class="qbr-grid" markdown="1">

<div class="qbr-card" markdown="1">

### Environment & project

Sign in, open your **project**, and confirm the **cluster** used for demos.

[Environment setup](labs/environment-setup.md){ .md-button }

</div>

<div class="qbr-card" markdown="1">

### Exposing applications

Overview of modules **01–06** and quick links into each exercise.

[Lab overview](labs/exposing-applications/index.md){ .md-button }

</div>

<div class="qbr-card" markdown="1">

### Official documentation

Procedures, UI paths, and glossary on the Cloudera Cloud Factory docs site.

[docs.taikun.cloud](https://docs.taikun.cloud/){ .md-button }

</div>

</div>

**Module order:** 01 DNS → 02 LoadBalancer → 03 Ingress basics → 04 Managed Apps → 05 CertManager → 06 Taikun Link → [Wrap-up](labs/workshop-wrap-up.md).

---

## Personalize examples (optional)

!!! tip "Optional: personalize code samples"
    Enter your assigned workshop username (for example `user001`) and click **UPDATE EXAMPLES** so snippets match your sandbox.

    <div class="username-input-container">
        <input type="text" id="user-username-input" placeholder="e.g., user001">
        <button id="user-username-save">UPDATE EXAMPLES</button>
        <button id="user-username-clear">RESET</button>
    </div>

    ```text title="Example placeholder"
    changed_user=USERNAME;
    ```

---

## Frequently asked questions

??? question "What is Cloudera Cloud Factory?"
    A platform for deploying and operating Kubernetes-centric workloads across public and private clouds from a unified control plane—so teams spend less time on undifferentiated plumbing and more on applications and data services.

??? question "What will I do in this workshop?"
    **Environment setup**, then six **Exposing applications** modules in order, aligned with [this documentation hub](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/Exposing_Applications/). Your facilitator demos in Cloud Factory; you use this site for structure and deep links.

??? question "Where is the full product documentation?"
    **[docs.taikun.cloud](https://docs.taikun.cloud/)** — use it for screenshots, edge cases, and topics outside this QBR lab slice.

??? question "Who do I contact for access issues?"
    Use the channel your facilitator shared. Do not post credentials or internal URLs in public forums or GitHub issues.

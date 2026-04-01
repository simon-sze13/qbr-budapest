# Instructor guide — QBR Cloudera Cloud Factory workshop

This guide covers local builds and publishing the participant-facing MkDocs site. Workshop **content** lives under [`../content/`](../content/); **configuration** lives in [`mkdocs/mkdocs.yml`](mkdocs/mkdocs.yml).

> [!TIP]
> **Workshop or POC environments** are arranged through your Cloudera account team or facilitator. Follow your internal process for tenant access, approvals, and duration—this public guide only documents the MkDocs site.

## Hands-on lab environment setup

Document tenant URLs, roles, and reset steps **in your private runbook** or facilitator notes; avoid putting internal hostnames or credentials in this repository.

## Publishing to GitHub Pages (public github.com)

The workflow [`.github/workflows/pages.yml`](../.github/workflows/pages.yml) runs on pushes to `main`. It installs [`mkdocs/requirements-ci.txt`](mkdocs/requirements-ci.txt), runs `mkdocs build --strict` from `instructor/mkdocs`, and deploys `build/` to **GitHub Pages**.

1. Repo **Settings → Pages → Source**: **GitHub Actions**.
2. **`site_url`** in `mkdocs.yml` is set to **https://simon-sze13.github.io/qbr-budapest/** (trailing slash required).

Optional CLI deploy:

```bash
cd instructor/mkdocs && pip install -r requirements.txt && mkdocs gh-deploy --force
```

## Local preview

```bash
cd instructor/mkdocs
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Open `http://127.0.0.1:8000`.

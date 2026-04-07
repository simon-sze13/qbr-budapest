# QBR — Cloudera Cloud Factory Workshop

**Live workshop site (MkDocs + Material):** [https://simon-sze13.github.io/qbr-budapest/](https://simon-sze13.github.io/qbr-budapest/)

This repository holds the **QBR Budapest** hands-on guide for **Cloudera Cloud Factory**. The GitHub **repository page** below shows this `README.md`; the **participant experience** is the Pages site above (orange theme, navigation, labs)—not this file.

## Workshop content

The site follows the same path as **[Exposing applications](https://docs.taikun.cloud/CloudWorks/Exposing_Applications/Exposing_Applications/)** on [docs.taikun.cloud](https://docs.taikun.cloud/):

| Step | Topic |
|------|--------|
| Home | Welcome, optional username helper, FAQs |
| Environment & project | Sign-in, project, cluster access |
| Exposing applications | Overview hub + modules **01–06** (DNS → LoadBalancer → Ingress → Managed Apps → CertManager → Taikun Link) |
| Workshop wrap-up | Discussion prompts and links |

Sources live under [`content/`](content/). Configuration: [`instructor/mkdocs/mkdocs.yml`](instructor/mkdocs/mkdocs.yml).

## Repository layout

| Path | Purpose |
|------|---------|
| [`content/`](content/) | Markdown for the published site |
| [`instructor/mkdocs/`](instructor/mkdocs/) | `mkdocs.yml`, `requirements.txt`, CI `requirements-ci.txt` |
| [`instructor/README.md`](instructor/README.md) | Build and publish notes |
| [`.github/workflows/pages.yml`](.github/workflows/pages.yml) | GitHub Actions → GitHub Pages |

## Run locally

```bash
cd instructor/mkdocs
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```

Open [http://127.0.0.1:8000](http://127.0.0.1:8000).

## GitHub Pages

1. **Source:** [Repository settings → Pages](https://github.com/simon-sze13/qbr-budapest/settings/pages) → **Build and deployment** → **GitHub Actions** (not “Deploy from a branch”).
2. Every push to `main` runs **Deploy MkDocs to GitHub Pages**. Approve the `github-pages` environment on first run if prompted.
3. Keep `site_url` in `mkdocs.yml` aligned with the live URL (trailing `/` required).

If **github.io** shows only plain README-style text, Pages is still serving from a **branch**; switch to **GitHub Actions** and re-run the workflow.

## Branding

- **Cloudera orange** (`#f96702`) and white: [`content/assets/stylesheets/extra.css`](content/assets/stylesheets/extra.css)
- Logo: [`content/assets/images/logo-cloudera-white.svg`](content/assets/images/logo-cloudera-white.svg)

## Contributing & license

Issues and PRs: [github.com/simon-sze13/qbr-budapest](https://github.com/simon-sze13/qbr-budapest). Do not commit secrets or internal-only URLs.

Licensed under **Apache License 2.0** — see [LICENSE](LICENSE).

# QBR — Cloudera Cloud Factory Workshop (MkDocs)

> **Participant site (styled workshop — open this in the browser):**  
> **[https://simon-sze13.github.io/qbr-budapest/](https://simon-sze13.github.io/qbr-budapest/)**
>
> This file is only the **GitHub repository README**. The repo page at [github.com/simon-sze13/qbr-budapest](https://github.com/simon-sze13/qbr-budapest) will always show this README below the file list — that is **not** the workshop website.

Public workshop guide for **QBR** demos of **Cloudera Cloud Factory**: agenda, prerequisites, hands-on lab modules, and links to full product documentation at [docs.taikun.cloud](https://docs.taikun.cloud/).

## What is inside

| Path | Description |
|------|-------------|
| [`content/`](content/) | Markdown sources for the participant-facing site |
| [`instructor/mkdocs/mkdocs.yml`](instructor/mkdocs/mkdocs.yml) | MkDocs + Material configuration |
| [`instructor/README.md`](instructor/README.md) | Instructor notes and local build commands |
| [`.github/workflows/pages.yml`](.github/workflows/pages.yml) | Builds and deploys the site to **GitHub Pages** |

## View the published site

Live site (GitHub Pages): **[https://simon-sze13.github.io/qbr-budapest/](https://simon-sze13.github.io/qbr-budapest/)**

Source repository: **[github.com/simon-sze13/qbr-budapest](https://github.com/simon-sze13/qbr-budapest)**

## Run locally

```bash
cd instructor/mkdocs
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```

Open `http://127.0.0.1:8000`.

## Publish to GitHub Pages

1. Push this project to [`simon-sze13/qbr-budapest`](https://github.com/simon-sze13/qbr-budapest) on the `main` branch.
2. **Critical:** In the repo go to **Settings → Pages → Build and deployment**. Set **Source** to **GitHub Actions** (not “Deploy from a branch”). If Source is **main** / **/ (root)**, GitHub uses Jekyll and the site will look like a plain **README** instead of the MkDocs workshop.
3. Open the **Actions** tab and confirm **Deploy MkDocs to GitHub Pages** completes (green). The first run may ask you to **approve** the `github-pages` environment under **Settings → Environments**.
4. Canonical URLs are in [`instructor/mkdocs/mkdocs.yml`](instructor/mkdocs/mkdocs.yml) (`site_url` must keep the trailing `/`).

### If you only see the README on github.io

- Pages is almost certainly set to **Deploy from a branch**. Switch it to **GitHub Actions**, re-run the workflow (**Actions → workflow → Run workflow**), then wait a minute and hard-refresh the site.

## Branding

- Theme uses **Cloudera orange** (`#f96702`) and **white** via [`content/assets/stylesheets/extra.css`](content/assets/stylesheets/extra.css).
- Header logo: [`content/assets/images/logo-cloudera-white.svg`](content/assets/images/logo-cloudera-white.svg) (from the upstream GOES template).

## Contributing

Open an issue or pull request for typos and improvements. Do not commit internal hostnames, credentials, or customer data.

## License

Licensed under the Apache License 2.0 — see [LICENSE](LICENSE).

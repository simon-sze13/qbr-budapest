# QBR — Cloudera Cloud Factory Workshop (MkDocs)

Public workshop guide for **QBR** demos of **Cloudera Cloud Factory**: agenda, prerequisites, hands-on lab modules, and links to full product documentation at [docs.taikun.cloud](https://docs.taikun.cloud/).

## What is inside

| Path | Description |
|------|-------------|
| [`content/`](content/) | Markdown sources for the participant-facing site |
| [`instructor/mkdocs/mkdocs.yml`](instructor/mkdocs/mkdocs.yml) | MkDocs + Material configuration |
| [`instructor/README.md`](instructor/README.md) | Instructor notes and local build commands |
| [`.github/workflows/pages.yml`](.github/workflows/pages.yml) | Builds and deploys the site to **GitHub Pages** |

## View the published site

After you enable GitHub Pages (see below), the site is served from:

`https://<your-github-user-or-org>.github.io/qbr-cloud-factory-workshop/`

Replace placeholders in [`instructor/mkdocs/mkdocs.yml`](instructor/mkdocs/mkdocs.yml):

- `site_url`
- `repo_url`
- `edit_uri` (optional)

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

1. Create a **public** repository on [github.com](https://github.com/new) (for example `qbr-cloud-factory-workshop`).
2. Push this project to the `main` branch.
3. In the repo: **Settings → Pages → Build and deployment → Source**: select **GitHub Actions**.
4. The **Deploy MkDocs to GitHub Pages** workflow runs on every push to `main`. The first run may require approving the `github-pages` environment.
5. Update `site_url` in `mkdocs.yml` to match the live URL (include trailing `/`), then push again.

## Branding

- Theme uses **Cloudera orange** (`#f96702`) and **white** via [`content/assets/stylesheets/extra.css`](content/assets/stylesheets/extra.css).
- Header logo: [`content/assets/images/logo-cloudera-white.svg`](content/assets/images/logo-cloudera-white.svg) (from the upstream GOES template).

## Contributing

Open an issue or pull request for typos and improvements. Do not commit internal hostnames, credentials, or customer data.

## License

Licensed under the Apache License 2.0 — see [LICENSE](LICENSE).

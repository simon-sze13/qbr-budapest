# Cloudera Cloud Factory — MCP workshop (MkDocs)

**Live site:** [https://simon-sze13.github.io/qbr-budapest/](https://simon-sze13.github.io/qbr-budapest/)

MkDocs workshop for the **custom Cloudera Cloud Factory MCP server**: build from **[skotnicky/cloudera-cloud-factory-mcp @ `app-latest`](https://github.com/skotnicky/cloudera-cloud-factory-mcp/tree/app-latest)**, configure **Robot User** credentials and **`api-latest.osc1.sjc.cloudera.com`**, connect **Cursor** over **stdio**, and run guided labs.

The **GitHub repo page** shows this README; the **workshop UI** is the Pages site above.

## Contents

| Topic | Site section |
|-------|----------------|
| MCP + CCF overview | [MCP overview](https://simon-sze13.github.io/qbr-budapest/mcp/) |
| Install / env / Cursor | Install, Configuration, Cursor & stdio |
| Tool catalog | Tool reference |
| Hands-on | Lab 1 — First connection, Lab 2 — Projects & catalogs |

Sources: [`content/`](content/) · Config: [`instructor/mkdocs/mkdocs.yml`](instructor/mkdocs/mkdocs.yml)

## Run locally

```bash
cd instructor/mkdocs
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

## GitHub Pages

**Settings → Pages → Source:** **GitHub Actions**. Push to `main` runs [`.github/workflows/pages.yml`](.github/workflows/pages.yml).

## Branding

Orange **`#FF550D`** in [`content/assets/stylesheets/extra.css`](content/assets/stylesheets/extra.css) · Logo in [`content/assets/images/`](content/assets/images/).

## License

[Apache License 2.0](LICENSE)

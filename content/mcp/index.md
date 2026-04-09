# MCP and Cloudera Cloud Factory

## Model Context Protocol (MCP)

[MCP](https://modelcontextprotocol.io/) is an open protocol for connecting AI assistants to **tools** and **data**. A **server** exposes named tools (with schemas); the **client** (for example **Cursor**) launches the server as a subprocess and talks over **stdio** by default.

## Cloudera Cloud Factory MCP server

The **[cloudera-cloud-factory-mcp](https://github.com/skotnicky/cloudera-cloud-factory-mcp/tree/app-latest)** project (fork of the Taikun MCP lineage) implements an MCP server in **Go**. It uses the **Taikun Go client** with **Robot User** access keys to call the **Cloudera Cloud Factory HTTP API**.

Typical use cases:

- List **projects**, **virtual clusters**, **catalogs**, and **applications** from chat.
- Drive **catalog** and **app install** flows with structured tool calls.
- **Deploy YAML** to Kubernetes projects, manage **kubeconfigs**, and inspect resources—within the scopes granted to your Robot User.

## app-latest environment

For the **latest application / API stack**, the default API host baked into the server is:

`api-latest.osc1.sjc.cloudera.com`

Override with **`TAIKUN_API_HOST`** if your facilitator gives a different host. Always use **non-production** tenants and **least-privilege** Robot Users in workshops.

## Branch to use

Workshop steps assume you work from:

**[https://github.com/skotnicky/cloudera-cloud-factory-mcp/tree/app-latest](https://github.com/skotnicky/cloudera-cloud-factory-mcp/tree/app-latest)**

```bash
git clone -b app-latest https://github.com/skotnicky/cloudera-cloud-factory-mcp.git
cd cloudera-cloud-factory-mcp
```

[Next: Prerequisites](prerequisites.md){ .md-button .md-button--primary }

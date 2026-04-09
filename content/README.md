---
hide:
  - toc
---
# Cloudera Cloud Factory — MCP workshop

This workshop walks you through the **custom Model Context Protocol (MCP) server** for **Cloudera Cloud Factory (CCF)**. You will build or install the binary, point it at the **app-latest** API (`api-latest.osc1.sjc.cloudera.com`), wire **Robot User** credentials, and connect **Cursor** (or another MCP client) over **stdio** so an AI assistant can call CCF tools safely.

**Reference repository (branch `app-latest`):** [github.com/skotnicky/cloudera-cloud-factory-mcp](https://github.com/skotnicky/cloudera-cloud-factory-mcp/tree/app-latest)

---

## Start here

<div class="qbr-grid" markdown="1">

<div class="qbr-card" markdown="1">

### MCP & CCF overview

What MCP is, how this server talks to CCF, and **app-latest**.

[MCP overview](mcp/index.md){ .md-button }

</div>

<div class="qbr-card" markdown="1">

### Install & configure

Clone **`app-latest`**, build with Go, set **`TAIKUN_*`** env vars.

[Install](mcp/install.md){ .md-button } [Configure](mcp/configuration.md){ .md-button }

</div>

<div class="qbr-card" markdown="1">

### Cursor connection

`mcp.json` + wrapper script for **stdio** transport.

[Cursor setup](mcp/cursor.md){ .md-button }

</div>

<div class="qbr-card" markdown="1">

### Tools & labs

Full tool list and guided exercises in the IDE.

[Tool reference](mcp/tools.md){ .md-button } [Lab 1](mcp/lab-01-connection.md){ .md-button }

</div>

<div class="qbr-card" markdown="1">

### Product docs

UI concepts, APIs, and operations on **docs.taikun.cloud**.

[docs.taikun.cloud](https://docs.taikun.cloud/){ .md-button }

</div>

</div>

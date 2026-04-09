# Cursor (and other MCP clients)

## stdio transport

The Cloudera Cloud Factory MCP server uses **stdio**: the client runs the binary as a subprocess and exchanges JSON-RPC over standard input/output.

## Option A — Wrapper script (recommended for workshops)

The **`app-latest`** tree includes **`scripts/run-user-robot-mcp.sh`**, which:

1. Loads **`$REPO_ROOT/.env.user-robot`**
2. Builds **`./cloudera-cloud-factory-mcp`** if missing
3. **`exec`**s the binary

**Cursor** `mcp.json` example (adjust paths to your machine):

```json
{
  "mcpServers": {
    "ccf-mcp-app-latest": {
      "command": "/absolute/path/to/cloudera-cloud-factory-mcp/scripts/run-user-robot-mcp.sh"
    }
  }
}
```

Copy from the repo template **[cursor-mcp-user-robot.example.json](https://github.com/skotnicky/cloudera-cloud-factory-mcp/blob/app-latest/cursor-mcp-user-robot.example.json)** and fix the **`command`** path.

Merge the `mcpServers` entry into your Cursor MCP settings (for example **Cursor Settings → MCP** or project `.cursor/mcp.json` per Cursor version).

## Option B — Inline `env` (Claude Desktop style)

You can pass env vars directly instead of a wrapper:

```json
{
  "mcpServers": {
    "ccf-mcp-app-latest": {
      "command": "/absolute/path/to/cloudera-cloud-factory-mcp/cloudera-cloud-factory-mcp",
      "env": {
        "TAIKUN_ACCESS_KEY": "your-key",
        "TAIKUN_SECRET_KEY": "your-secret",
        "TAIKUN_API_HOST": "api-latest.osc1.sjc.cloudera.com"
      }
    }
  }
}
```

!!! tip "Restart Cursor"
    After editing MCP config, **reload** or restart Cursor so it spawns a fresh server process.

[Next: Tool reference](tools.md){ .md-button .md-button--primary }

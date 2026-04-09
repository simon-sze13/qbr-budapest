# Configuration (Robot User + app-latest API)

The server uses **legacy `TAIKUN_*` variable names** expected by the Go API client.

## Required variables

| Variable | Purpose |
|----------|---------|
| `TAIKUN_ACCESS_KEY` | Robot User access key |
| `TAIKUN_SECRET_KEY` | Robot User secret key |

## API host (app-latest)

Default in code: **`api-latest.osc1.sjc.cloudera.com`**

Set explicitly if needed:

```bash
export TAIKUN_API_HOST="api-latest.osc1.sjc.cloudera.com"
```

## Optional

| Variable | When to set |
|----------|-------------|
| `TAIKUN_DOMAIN_NAME` | Only if your environment requires an explicit domain name |

## Example `.env` file

Create a file (for example **`.env.user-robot`**) in the repo root—**do not commit it**:

```bash
TAIKUN_ACCESS_KEY=your-robot-user-access-key
TAIKUN_SECRET_KEY=your-robot-user-secret-key
TAIKUN_API_HOST=api-latest.osc1.sjc.cloudera.com
# TAIKUN_DOMAIN_NAME=only-if-required
```

The repo’s **`scripts/run-user-robot-mcp.sh`** script `source`s **`.env.user-robot`** and then execs the binary (see [Cursor setup](cursor.md)).

## Refresh client

After changing env vars, restart the MCP server (or use the **`refresh-taikun-client`** tool from a connected client if available in your build).

[Next: Cursor & stdio](cursor.md){ .md-button .md-button--primary }

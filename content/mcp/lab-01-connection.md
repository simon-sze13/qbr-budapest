# Lab 1 — First connection

## Goal

Confirm **Cursor** (or your client) starts the **CCF MCP server** and can invoke at least one **read-only** tool against **app-latest**.

## Steps

1. Complete [Install](install.md) and [Configuration](configuration.md); verify **`.env.user-robot`** exists if you use [run-user-robot-mcp.sh](https://github.com/skotnicky/cloudera-cloud-factory-mcp/blob/app-latest/scripts/run-user-robot-mcp.sh).
2. Add the MCP server to Cursor per [Cursor setup](cursor.md).
3. Reload **MCP** in Cursor and open the **MCP tools** panel; confirm **`ccf-mcp-app-latest`** (or your server name) is connected without errors.
4. In chat, ask the assistant to run **`list-projects`** or **`catalog-list`** with conservative filters your facilitator approves.
5. Inspect the JSON response: you should see **projects** or **catalogs** your Robot User can access.

## Success criteria

- [ ] MCP server process starts (no immediate crash / auth error in logs).
- [ ] At least one **list** tool returns **200-style** success payload from the API.

## Troubleshooting

- **Auth errors:** Recheck `TAIKUN_ACCESS_KEY` / `TAIKUN_SECRET_KEY` and `TAIKUN_API_HOST`.
- **Scope errors:** Robot User lacks permission for that tool—see [Prerequisites](prerequisites.md).
- **Path errors:** Use **absolute paths** in `mcp.json` for `command`.

[Lab 2: Projects & catalogs](lab-02-projects-catalogs.md){ .md-button .md-button--primary }

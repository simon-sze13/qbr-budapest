# Prerequisites

## On your laptop

- **Go 1.24+** if you build from source ([install](https://go.dev/dl/)).
- **Git** to clone the `app-latest` branch.
- **Cursor** (or another MCP-capable client) for [stdio setup](cursor.md).
- **Bash** for the optional `scripts/run-user-robot-mcp.sh` wrapper (macOS / Linux).

## In Cloudera Cloud Factory

- A **Robot User** with **access key** and **secret key** (from your org / facilitator).
- **API scopes** that match the tools you plan to run (list projects, install apps, etc.). If a tool fails with a scope error, ask your admin to widen Robot User permissions or use a different user.
- Awareness of **which organization and projects** are in scope for the workshop (avoid production).

## Security

!!! warning "Secrets"
    Never commit `.env.user-robot`, real keys, or kubeconfigs to Git. Keep env files **local** and **gitignored**.

[Next: Install & build](install.md){ .md-button .md-button--primary }

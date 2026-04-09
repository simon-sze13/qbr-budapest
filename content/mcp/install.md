# Install and build

## Clone `app-latest`

```bash
git clone -b app-latest https://github.com/skotnicky/cloudera-cloud-factory-mcp.git
cd cloudera-cloud-factory-mcp
```

## Build the binary

```bash
go build -o cloudera-cloud-factory-mcp .
```

The executable **`cloudera-cloud-factory-mcp`** speaks MCP on **stdin/stdout** when run without extra arguments (see upstream [README](https://github.com/skotnicky/cloudera-cloud-factory-mcp/blob/app-latest/README.md) for release binaries if you prefer not to build).

## Optional: install to PATH

```bash
sudo mv cloudera-cloud-factory-mcp /usr/local/bin/
```

## Smoke test (stdio)

With [environment variables](configuration.md) exported in the shell:

```bash
./cloudera-cloud-factory-mcp
```

The process waits for MCP messages on stdio; **Ctrl+C** to exit. Cursor will spawn this process for you—manual run is mainly for debugging.

[Next: Configuration](configuration.md){ .md-button .md-button--primary }

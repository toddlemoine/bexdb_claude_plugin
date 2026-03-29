# BexDB Claude Code Plugin

Claude Code plugin that installs the [BexDB](https://bexdb.io) MCP server.

## Installation

```
claude plugin add github:toddlemoine/bexdb_claude_plugin
```

During installation, Claude Code will prompt you for:

- **API token** — your BexDB API token (stored securely in your system keychain). Leave blank if `BEXDB_API_TOKEN` is already set in your environment.
- **Config file path** — path to a BexDB config file containing your API token (optional alternative to entering it directly).

## Configuration

The MCP server reads credentials in this order of precedence (handled by the server itself):

1. `BEXDB_API_TOKEN` environment variable
2. Config file at the path specified by `BEXDB_CONFIG_FILE`

If `BEXDB_API_TOKEN` is already exported in your shell environment, no configuration is needed during install.

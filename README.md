# agents-marketplace

All information around the justtrack-platform MCP.

This repository is a [Claude Code plugin marketplace](https://docs.claude.com/en/docs/claude-code/plugin-marketplaces)
that installs the justtrack platform MCP server (`https://mcp.justtrack.io/mcp`) into your agent.

## Installation

In Claude Code, add this repository as a marketplace and install the plugin:

```
/plugin marketplace add justtrackio/agents-marketplace
/plugin install justtrack-platform@justtrack
```

Restart Claude Code afterwards so the MCP server is picked up, then verify it with `/mcp`.

## Contents

| Plugin | Description |
| --- | --- |
| [`justtrack-platform`](plugins/justtrack-platform) | Registers the justtrack platform MCP server (`https://mcp.justtrack.io/mcp`) |

## Repository layout

```
.claude-plugin/marketplace.json                       # marketplace manifest listing all plugins
plugins/justtrack-platform/.claude-plugin/plugin.json # plugin manifest with the MCP server definition
```

To add another plugin, create a new directory under `plugins/` containing a
`.claude-plugin/plugin.json` and reference it from `.claude-plugin/marketplace.json`.

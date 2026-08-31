# justtrack agent marketplace

Install the justtrack platform MCP plugin from this repository.

## Claude Code

```sh
claude plugin marketplace add justtrackio/agents-marketplace
claude plugin install justtrack-platform@justtrack
```

Run `/mcp` to sign in with OAuth and check the connection.

## Codex

```sh
codex plugin marketplace add justtrackio/agents-marketplace
codex plugin add justtrack-platform@justtrack
```

Start a new Codex session after installation.

Both clients connect to `https://mcp.justtrack.io/mcp` using Streamable HTTP and
discover OAuth from the server. No token is stored in this repository.

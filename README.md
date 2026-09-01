# justtrack agent marketplace

Install the justtrack MCP plugin from this repository.

## Claude Code

### Desktop app

1. Click **+** next to the prompt, then select **Plugins** and **Browse plugins**.
2. Select **Personal**, then click **+** (**Add marketplace**).
3. Enter `justtrackio/agents-marketplace` as the **URL**, keep
   **Sync automatically** enabled, and click **Sync**.
4. Select **agents-marketplace**, find **justtrack**, and click **+**
   (**Install**).
5. Open **justtrack**, then click **Connect** under **Connectors** and complete
   OAuth in the browser.

### CLI

```sh
claude plugin marketplace add justtrackio/agents-marketplace
claude plugin install justtrack@justtrack
```

Run `/mcp` to sign in with OAuth and check the connection.

## Codex

### Desktop app

1. Open **Plugins** from the sidebar.
2. Click **Add**, then select **Add a marketplace**.
3. Enter `justtrackio/agents-marketplace` as the **Source**, leave **Git ref**
   empty to use `main`, and click **Add marketplace**.
4. Open **justtrack** and click **Install plugin**.
5. Start a new task and complete OAuth in the browser when prompted.

### CLI

```sh
codex plugin marketplace add justtrackio/agents-marketplace
codex plugin add justtrack@justtrack
```

Start a new Codex session after installation.

Both clients connect to `https://mcp.justtrack.io/mcp` using Streamable HTTP and
discover OAuth from the server. No token is stored in this repository.

<p align="center">
  <a href="https://justtrack.io/">
    <img src="./plugins/justtrack/assets/icon.png" alt="justtrack" width="72">
  </a>
</p>

<h1 align="center">justtrack agent marketplace</h1>

<p align="center">
  Connect Claude Code and Codex to justtrack through MCP.
</p>

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

---

<p align="center">
  <a href="https://justtrack.io/">Website</a> ·
  <a href="https://www.linkedin.com/company/justtrack/">LinkedIn</a> ·
  <a href="https://www.instagram.com/justtrack.io/">Instagram</a> ·
  <a href="https://justtrack.io/security/">Security</a> ·
  <a href="https://justtrack.io/privacy-notice/">Privacy</a> ·
  <a href="https://justtrack.io/terms-of-service/">Terms</a> ·
  <a href="https://justtrack.io/imprint/">Imprint</a>
</p>

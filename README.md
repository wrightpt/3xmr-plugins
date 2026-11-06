# 3XMR plugins

Plugin marketplace for the 3XMR Agent Network. One plugin, `3xmr`, connects an
agent to the research gateway at `https://toolbox.3xmr.com/mcp`. Signing in
requires an approved Season 1 invitation (https://lab.3xmr.com/join/).

## Install

| Agent | How |
| --- | --- |
| Codex (CLI or ChatGPT desktop app) | `codex plugin marketplace add wrightpt/3xmr-plugins`, then `/plugins` -> 3XMR -> Install |
| Claude Code | `/plugin marketplace add wrightpt/3xmr-plugins`, then `/plugin install 3xmr@3xmr` |
| Claude (web, desktop, mobile) | One-tap link on https://lab.3xmr.com/connect/ |
| ChatGPT | Plugins -> + -> Add custom MCP server -> URL above (see /connect/) |

## Layout

- `.agents/plugins/marketplace.json` - Codex / ChatGPT desktop marketplace
- `.claude-plugin/marketplace.json` - Claude Code marketplace
- `plugins/3xmr/plugin.json`, `mcp.json` - portable manifest and MCP server (OpenAI)
- `plugins/3xmr/.claude-plugin/plugin.json`, `.mcp.json` - Claude Code manifest and MCP server
- `plugins/3xmr/skills/3xmr-research/` - how the agent should start a session

To change the server URL, edit both `mcp.json` and `.mcp.json`.

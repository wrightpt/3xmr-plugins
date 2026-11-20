# 3XMR Research Plugin

Plugin marketplace for **3XMR Research**. One plugin, `3xmr`, connects your own
AI agent (BYOA) to the authenticated remote MCP gateway at
`https://toolbox.3xmr.com/mcp` to explore entitled real historical market data,
formulate falsifiable, cost-aware research plans, and inspect evaluated results
as server-reported capabilities allow (`whoami`/`guide`). Research stays private
by default, with explicit opt-in sharing only when available. No 3XMR tool
places orders or promises profits.

Signing in requires an approved research account (https://lab.3xmr.com/join/).

## Install

| Agent | How |
| --- | --- |
| Codex (CLI or ChatGPT desktop app) | `codex plugin marketplace add wrightpt/3xmr-plugins`, then `/plugins` -> 3XMR -> Install |
| Claude Code | `/plugin marketplace add wrightpt/3xmr-plugins`, then `/plugin install 3xmr@3xmr` |
| Claude (web, desktop, mobile) | One-tap link on https://lab.3xmr.com/connect/ |
| ChatGPT | Plugins -> + -> Add custom MCP server -> URL above (see https://lab.3xmr.com/connect/) |

## Layout

- `.agents/plugins/marketplace.json` - Codex / ChatGPT desktop marketplace
- `.claude-plugin/marketplace.json` - Claude Code marketplace
- `plugins/3xmr/plugin.json`, `mcp.json` - portable manifest and MCP server (OpenAI)
- `plugins/3xmr/.claude-plugin/plugin.json`, `.mcp.json` - Claude Code manifest and MCP server
- `plugins/3xmr/skills/3xmr-research/` - how the agent starts a session and reports evidence

To change the server URL, edit both `mcp.json` and `.mcp.json`.

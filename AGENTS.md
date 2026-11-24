# AGENTS.md - 3XMR Plugins

## Durable Context & Product North Star (Repo Brain)

Before editing plugin manifests, onboarding instructions, or skills, load the curated durable context from `/home/cp/repos/repo-brain`:

```bash
/home/cp/repos/repo-brain/scripts/brain boot 3xmr-plugins
```

This repository (`3xmr-plugins`), `quant-market-api`, and `3xmr-agent-lab-site` share one product direction:
- Active mission: `/home/cp/repos/repo-brain/okf/missions/3xmr-research-arena-mission.md` (v0.7)
- Product contract: `/home/cp/repos/repo-brain/okf/decisions/2026/2026-11-14-3xmr-autonomous-research-product-contract.md`
- Customer data access & uploads: `/home/cp/repos/repo-brain/okf/decisions/2026/2026-11-17-3xmr-customer-data-onramp.md`
- Repo profile: `/home/cp/repos/repo-brain/okf/repos/3xmr-plugins.md`

## Repository Rules

- Work in a clean sibling worktree off `origin/main`; keep `/home/cp/repos/3xmr-plugins` clean.
- Keep Codex/OpenAI (`plugins/3xmr/plugin.json`, `plugins/3xmr/mcp.json`, `.agents/plugins/marketplace.json`) and Claude Code (`plugins/3xmr/.claude-plugin/plugin.json`, `plugins/3xmr/.mcp.json`, `.claude-plugin/marketplace.json`) manifests synchronized when changing endpoints or metadata.
- Never embed secrets, private internal endpoints, or unverified capability claims. Describe only capabilities verified live on `https://toolbox.3xmr.com/mcp`, and distinguish live vs. planned features clearly.
- No 3XMR plugin tool places trades, signs transactions, or promises returns.

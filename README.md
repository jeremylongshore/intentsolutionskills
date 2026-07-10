# agent-skills

Curated agent skills from [Tons of Skills](https://tonsofskills.com) — the Claude Code plugins marketplace (450+ plugins, 3,000+ skills) — packaged for one-command install with [`npx skills`](https://github.com/vercel-labs/skills).

```bash
# install a specific skill
npx skills add jeremylongshore/agent-skills --skill databricks-cost-leak-hunter

# or browse everything in this repo
npx skills add jeremylongshore/agent-skills
```

Skills follow the [Agent Skills](https://agentskills.io) standard and work with Claude Code, Codex, Cursor, and Gemini CLI.

## Skills

| Skill | What it does |
| ----- | ------------ |
| [`databricks-cost-leak-hunter`](skills/databricks-cost-leak-hunter) | Hunt down Databricks cost leaks — wasted DBUs, idle clusters, oversized SQL warehouses, untagged runaway spend — and produce a FinOps cost report. Ships with reference docs, helper scripts, and a behavioral eval spec. |
| [`wallet`](skills/wallet) | Agent Wallet — create a policy-bounded wallet the agent can use for EVM transfers, swaps, and contract calls without exposing private keys. |

More are on the way — the top-graded skills from the marketplace are being rolled out here. The full catalog lives at [tonsofskills.com](https://tonsofskills.com) and installs as Claude Code plugins via:

```
/plugin marketplace add jeremylongshore/claude-code-plugins
```

## Notes

- Canonical source: [`jeremylongshore/claude-code-plugins-plus-skills`](https://github.com/jeremylongshore/claude-code-plugins-plus-skills) — skills here are published snapshots of the marketplace copies (this cut: `7ffa06a3d`).
- `databricks-cost-leak-hunter` optionally pairs with the `databricks` CLI and the pack's workspace MCP server for live-workspace probes; without them it still guides the full manual audit path.
- License: MIT (per-skill frontmatter is authoritative; the `wallet` skill predates this README and carries its own terms in-skill).

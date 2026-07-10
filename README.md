# intentsolutionskills

Intent Solutions' **best skills only** — the top-graded, production-hardened cut of the [Tons of Skills](https://tonsofskills.com) marketplace (450+ plugins, 3,000+ skills), packaged for one-command install with [`npx skills`](https://github.com/vercel-labs/skills). Every skill here is hand-picked: featured or A-grade under the marketplace's 100-point validator, shipped with its references, scripts, and eval spec.

```bash
# install a specific skill
npx skills add jeremylongshore/intentsolutionskills --skill databricks-cost-leak-hunter

# or browse everything in this repo
npx skills add jeremylongshore/intentsolutionskills
```

Skills follow the [Agent Skills](https://agentskills.io) standard and work with Claude Code, Codex, Cursor, and Gemini CLI.

## Skills

| Skill | What it does |
| ----- | ------------ |
| [`databricks-cost-leak-hunter`](skills/databricks-cost-leak-hunter) | Hunt down Databricks cost leaks — wasted DBUs, idle clusters, oversized SQL warehouses, untagged runaway spend — and produce a FinOps cost report. Ships with reference docs, helper scripts, and a behavioral eval spec. |

More are on the way — the marketplace's best are being rolled out here on a curated, reviewed cadence.

## Updating

Skills install as snapshots — they do not change under you. Pull the latest published versions any time with:

```bash
npx skills update
```

Repo-side, each skill is a reviewed snapshot of its marketplace source (pinned by commit in the publish notes); refreshes land here when the source skill ships a new version. The full catalog lives at [tonsofskills.com](https://tonsofskills.com) and installs as Claude Code plugins via:

```
/plugin marketplace add jeremylongshore/claude-code-plugins
```

## Notes

- Canonical source: [`jeremylongshore/claude-code-plugins-plus-skills`](https://github.com/jeremylongshore/claude-code-plugins-plus-skills) — skills here are published snapshots of the marketplace copies (this cut: `7ffa06a3d`).
- `databricks-cost-leak-hunter` optionally pairs with the `databricks` CLI and the pack's workspace MCP server for live-workspace probes; without them it still guides the full manual audit path.
- License: MIT (per-skill frontmatter is authoritative).

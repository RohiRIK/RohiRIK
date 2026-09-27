<img src="./assets/avatar.jpg" width="140" alt="Rohi Rikman" align="right" />

# Rohi Rikman

I build security and infrastructure tooling for Microsoft 365 and cloud tenants, and I publish what broke while building it.

Blog: [CloudJourneyBlog](https://CloudJourneyBlog.rohi-lab.org) — security, automation, systems.

## What I work on

I build tools for AI coding agents, and I ship them across many agent hosts at once. The M365 security work is the domain I apply inside that frame.

**microsoft-graph-security** (private for now) — Microsoft 365 security investigation skills, packaged once for many agents. Claude Code, Antigravity, Goose, Pi, OpenCode, and anything else that speaks MCP, with a `plugins/` directory for Claude Code, Pi and Hermes, an `antigravity/` adapter and a `goose/` YAML. `INSTALL-AGENTS.md` documents 47 agent hosts, each with the command, the verification, the rollback, and the honest limits. Read-only by default. Write tools sit behind a backend opt-in, destructive writes need `confirm: true`, and every investigation opens by naming the tenant from `gateway://session`. Python, MIT. Created this month.

**[OpenLtm](https://github.com/RohiRIK/OpenLtm)** — long-term memory plugin for Claude Code. Semantic search over what I have already worked out, context injected back into the session, and learning from the session so the next one starts further along. The only repo I work on daily, and it is maintained against real publishing infrastructure now — ClawHub, npm, OpenClaw packaging, and a CI check that fails on published-version drift. TypeScript, MIT. It is the memory layer behind the other things here.

**Omarchy bar widgets** — a small desktop stack in QML for observing and controlling what agents actually do.

- [omarchy-agent-monitor](https://github.com/RohiRIK/omarchy-agent-monitor) — AI coding agent limits, activity and model usage, in the bar. Has a marketplace preview. No license file.
- [omarchy-docker-monitor](https://github.com/RohiRIK/omarchy-docker-monitor) — host metrics, Compose groups, container pages, logs and controls, for Omarchy Quattro. Docker collection is bounded, and container output renders as plain text. Released today. MIT.
- [rohi.network](https://github.com/RohiRIK/rohi.network) — a clone of Omarchy's stock `omarchy.network` widget with two additions: a public-IPv4 lookup and an in-panel IP settings editor. The README screenshots are rendered from synthetic data, and I made the README safe to publish before the repo went out. No license file. ([omarchy-network-settings](https://github.com/RohiRIK/omarchy-network-settings) is the archived predecessor; it continues as this repo.)
- [omarchy-plugin-lab](https://github.com/RohiRIK/omarchy-plugin-lab) — lifecycle, health and marketplace feedback for the shell plugins I build. Lifecycle stage comes from git, GitHub, and the omarchy-plugin-marketplace submission and verification issues. Health comes from CI, local test results, manifest validation, uncommitted work, and a bar still running older code than the working copy. The "Fix with agent" action opens my agent in the plugin working copy with every flagged issue, the failing CI run and the marketplace review comments, and tells it to commit locally and ask before pushing, tagging, commenting or submitting. Python, MIT. Created today.

**[hermes-telemetry](https://github.com/RohiRIK/hermes-telemetry)** — budget enforcement and observability plugin for Hermes Agent, which stops runaway cost before it happens. A fork — I contribute upstream rather than only shipping my own. MIT.

**[skills](https://github.com/RohiRIK/skills)** — my everyday agent skills library, for Claude Code, opencode and friends. TypeScript, MIT.

**What went quiet.** [argus](https://github.com/RohiRIK/argus) — self-hosted, Dockerized notification and reporting for Microsoft 365, for IT admins and security teams — is the repo people find first and the one I have not touched since June. It has no license file, so read it before you depend on it. [aegis-security-agent](https://github.com/RohiRIK/aegis-security-agent) (no license, no description) and [corporate-on-demand](https://github.com/RohiRIK/corporate-on-demand) (no license) are the same. I would rather tell you that here than let the last commit date be the only signal.

**Not my repositories, still my week.** Since 2026-08-28: 100 pull requests and 22 issues, 90 of those PRs in my own homelab. Outside it, 5 to [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent), 8 to [omacom/omarchy-plugin-marketplace](https://github.com/omacom/omarchy-plugin-marketplace), 4 to nujovich/hermes-telemetry, 2 to [omacom/omarchy](https://github.com/omacom/omarchy), 1 to bobeff/open-source-games. Most of the ones filed against my own estate are security findings, not features.

Also on the account: [fleetwatch](https://github.com/RohiRIK/fleetwatch) (Intune device inventory — 34 open issues), [synapse-mcp](https://github.com/RohiRIK/synapse-mcp) (tenant-isolated MCP gateway, stdio upstream and authenticated SSE downstreams, no license), [omarchy-nanoclaw](https://github.com/RohiRIK/omarchy-nanoclaw) (unofficial NanoClaw plugin for Omarchy), [cloudjourneyblog](https://github.com/RohiRIK/cloudjourneyblog), and the older PowerShell and enterprise MS scripts.

## Stack

TypeScript · Python · Next.js · PostgreSQL · Docker · M365 · Azure · GCP · Claude Code · MCP · QML · PowerShell

## Elsewhere

- Blog — https://CloudJourneyBlog.rohi-lab.org
- README.md in this repo is mine. If something here is wrong, open an issue or send a note.

<!---
RohiRIK/RohiRIK is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
-->

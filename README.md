# ai-arsenal

A curated, opinionated collection of AI skills, agent frameworks, self-hosted tools, and awesome lists. Seeded from verified research (October 2026), maintained daily. No marketing fluff: every entry earned its place or it would not be here.

Built for a local-first homelab operator: Mac mini, Linux boxes (whitebox, redbox), NAS, Ollama on whitebox. If an entry needs cloud, it says so.

## Categories

- [Agent skills](skills-agent.md) - drop-in skills for Claude Code, Codex, and other agents
- [Awesome lists](awesome-lists.md) - the meta-list: curated lists worth checking before building anything
- [Agent frameworks](frameworks-agents.md) - orchestration, memory, supervision, browser agents
- [Self-hosted AI](selfhosted-ai.md) - run it on your own hardware
- [Local LLM](local-llm.md) - Ollama, models, inference notes
- [Dev tools](dev-tools.md) - recon, document conversion, design assets
- [Media tools](media-tools.md) - compression, downloads, Mac utilities
- [Security](security.md) - pentest methodology, recon kit, RF tools (authorized work only)
- [Prompts and workflows](prompts-workflows.md) - the few prompt resources that are not hype

## Daily maintenance

This repo is maintained by a daily worker. See [MAINTENANCE.md](MAINTENANCE.md) for the spec and [_maintain/DAILY_PROMPT.md](_maintain/DAILY_PROMPT.md) for the exact prompt the worker runs. Findings land in [daily-log.md](daily-log.md).

Rules the maintainer follows:
1. Every link gets HTTP-checked; dead ones are flagged, then removed after 7 days dead.
2. New releases on listed repos get a one-line note in the daily log.
3. New awesome lists found via search get evaluated and either added or rejected with a reason.
4. One-line descriptions only. Opinionated, no fluff.

## Publishing

This is a local git repo. To publish: `gh auth login`, then add the remote and push. Nothing here is secret, but review before making it public.

Last updated: 2026-10-02

# Agent frameworks

Orchestration, memory, supervision, and browser agents. Ordered by relevance to the current routing and agent-ops work.

- [jev-ultrafast](https://github.com/browser-use/browser-use) - fast browser agent built on TypeSafe's Jev decision model; the documented ~7s demo is real (small-sample caveat). Needs a Jev API key, metered but cheap. Relevant to browser-automation lanes.
- [Foreman](https://github.com/thruwire/foreman) - supervisor layer that judges coding-agent steps at checkpoints. Directly relevant to the agent supervision and routing work.
- [OpenViking](https://github.com/ruchuteam/openviking) - unified agent memory, knowledge, and skills database with a filesystem paradigm and tiered loading. An interesting answer to the context-management problem.
- laya - free local decision engine, 24 to 29ms inference. Worth watching as a local alternative for routing decisions. Canonical link pending.
- google/ax - Google's open agent orchestration runtime. Canonical link pending.
- hindsight - MIT-licensed agent memory with image support. Canonical link pending.
- paperclip (org-chart agent management) - budgets, tickets, and approval gates for agents. Conceptually adjacent to the agent-ops thinking; note the name collision with the Paperclip worklog beat, which is a different thing. Canonical link pending.
- OpenMAIC - Tsinghua AI classroom generated from one prompt. Interesting demo of single-prompt system generation. Canonical link pending.
- [agent-monitor](https://github.com/a0s/agent-monitor) - live tree of every Codex and Claude Code session, subagent, and teammate in a repo, with model, effort, task, and status. Started as the agent-tree monitor in harness-supervisor (the "agent tree" TUI from the @polydao screenshots). Reads transcripts and processes, nothing installed into the project. `brew install a0s/agent-monitor/agent-monitor`, then run `agent-monitor` in a project dir. Directly useful for watching multi-agent runs.

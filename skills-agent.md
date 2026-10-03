# Agent skills

Drop-in skills for Claude Code, Codex, Cursor, and other agents. Pure knowledge and methodology files; no executables.

- [claude-red](https://github.com/SnailSploit/Claude-Red) - 78 red-team methodology SKILL.md files (SQLi, wireless, AD, EDR evasion, exploit dev, recon). MIT. Strongest single find: one git clone arms the pentest team's study material. Authorized engagements only.
- [ponytail](https://github.com/DietrichGebert/ponytail) - Claude Code plugin that makes the agent act like a lazy senior dev. Fights over-engineering; published benchmarks show 80 to 94 percent less code vs baseline (author's own numbers, treat as directional).
- [mattpocock/skills](https://github.com/mattpocock/skills) - Matt Pocock's 37 agent skills, including the viral grill-me skill.
- [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) - 163 research skills across 78 databases.
- [anthropics/skills](https://github.com/anthropics/skills) - official Agent Skills repo: SKILL.md exemplars, production document skills, skill-creator, and the Agent Skills spec.
- [firecrawl/anydoc skill](https://github.com/firecrawl/anydoc) - ships as an agent skill (`npx skills add firecrawl/anydoc`); teaches agents to convert any document to Markdown.

Skill format note: most of these follow the agentskills.io SKILL.md convention (name and description frontmatter, UTF-8, LF line endings). Drop them in `~/.claude/skills/` or the equivalent for your agent.

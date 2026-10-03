# Daily log

## 2026-10-02: repo created

- Initialized ai-arsenal as a local git repo at ~/workspace/ai-arsenal.
- Seeded from the Instagram research file (25 posts reviewed, 15 marked worth implementing): claude-red, ponytail, jev-ultrafast, OpenViking, Foreman, Paperless-ngx, Open WebUI, Nhost, Penpot, Ollama plus the abliterated Qwen note, RustScan, Arjun, Katana, GoSpider, ParamSpider, Anydoc, Aria-Icons, Squoosh, Cobalt, MacTap, Textream, Zsky AI, GQRX, GNU Radio, Aircrack-NG, the browser extension recon kit, and the honest prompt resources.
- Verified 37 URLs live via HTTP status (two GitHub redirects resolved to their canonical targets: awesomelistsio/awesome-prompt-engineering to brandonhimpfen/awesome-prompt-engineering, f/awesome-chatgpt-prompts to f/prompts.chat).
- 15 awesome lists promoted to awesome-lists.md; 8 alternates held for evaluation.
- 9 entries marked "canonical link pending" for the daily job to resolve: Matt Pocock's 37 skills, K-Dense-AI scientific-agent-skills, Anthropic cybersecurity skills, laya, google/ax, hindsight, paperclip (agent-ops), OpenMAIC, Open Notebook, Strix, Open-kritt, VoiceStudio, Aria-Icons, and the five recon tools (RustScan, Arjun, Katana, GoSpider, ParamSpider).
- Not published to GitHub (gh CLI not authenticated). Push-ready: `gh auth login`, add remote, push.

## 2026-10-03: daily maintenance

- Link health: 34 URLs checked (all *.md except _maintain/), all returned HTTP 200. Zero dead links. Nothing flagged, nothing removed.
- New releases (Atom feeds, newer than 2026-10-02): DietrichGebert/ponytail v4.10.3 (2026-10-03): per-project ponytail mode, no more mode fighting across sessions; Codex yellow warning fix. danielmiessler/fabric v1.4.507 (2026-10-03): minor fix, clearer error when binary name is used as pattern fallback. Also noted, released 2026-10-02: ollama/ollama v0.35.1, adds Cloudflare Clef (27B) and Clef Flash (9B) decision models via /v1/systemone.
- Weekly rotation day 6 (awesome prompt engineering): evaluated held candidate calebvbi/awesome-prompt-engineering, rejected (0 stars, last push 2026-06-12, stale). Added NirDiamant/Prompt_Engineering to awesome-lists.md (22 techniques as runnable notebooks, 7.9k stars, pushed 2026-10-01): the learn-by-doing complement to the dair-ai reference.
- Pending links: all 18 resolved and pinned as verified markdown links. skills-agent.md: mattpocock/skills, K-Dense-AI/scientific-agent-skills, anthropics/skills. frameworks-agents.md: NandhaKishorM/laya, google/ax, vectorize-io/hindsight, paperclipai/paperclip, THU-MAIC/OpenMAIC. selfhosted-ai.md: lfnovo/open-notebook, usestrix/strix, Kritt-ai/open-kritt. local-llm.md: debpalash/VoiceStudio. dev-tools.md: LeulAria/Aria-Icons, bee-san/RustScan (canonical; old RustScan org path now redirects), s0md3v/Arjun, projectdiscovery/katana, jaeles-project/gospider, devanshbatham/ParamSpider. No placeholders remain in category files.
- New research: no ig-saved-weekly-research files newer than the 2026-10-02 seed fold. Nothing to merge.

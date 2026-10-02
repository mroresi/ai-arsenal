# Maintenance spec

The ai-arsenal repo is maintained by a daily worker running [_maintain/DAILY_PROMPT.md](_maintain/DAILY_PROMPT.md) verbatim. This file is the human-readable spec behind that prompt.

## Daily checks

1. **Link health.** HTTP-check every link in every category file (HEAD or GET, 20s timeout, browser user-agent). Record the status code. Any link that fails gets a `DEAD <date>` flag inline next to it. A link dead for 7 consecutive days is removed; the removal is noted in daily-log.md.
2. **New releases.** For each GitHub repo linked, check its releases page (or the Atom feed at `https://github.com/<owner>/<repo>/releases.atom`). If a release is newer than the last recorded check, add a one-line note to daily-log.md: repo, version, one-line summary of what changed.
3. **New awesome lists.** Run a web search for each of these, once per week on rotation (not all every day): awesome claude skills, awesome AI agents, awesome local LLM, awesome self-hosted AI, awesome MCP servers, awesome prompt engineering. Evaluate any new list found: is it curated (not a star farm), active (commits in the last 90 days), and relevant? Add it to awesome-lists.md or reject it with a one-line reason in daily-log.md.
4. **Pending canonical links.** Several entries are marked "canonical link pending." The worker searches for each one's canonical repo, verifies it live, and replaces the placeholder with a real link.
5. **Seed from new research.** If new Instagram research files appear in `~/workspace/your_files/ig-saved-weekly-research-*.md`, fold their ✅ items into the matching categories.

## Log and commit

- Append every finding to daily-log.md under a dated heading. Even "no changes" gets one line; silence is not evidence the job ran.
- Update the "Last updated" date in README.md.
- Commit with message `daily: YYYY-MM-DD - <one-line summary>`. Push only if a remote is configured; never invent one.

## Rules that do not change

- One-line descriptions. Opinionated, no marketing fluff.
- No em dashes in any file (commas, colons, periods).
- Every link verified live before it is added. No invented URLs, ever.
- Local-first bias: if an entry needs cloud, it says so.
- The security boundary stands: authorized engagements only; nothing in security.md gets a dual-use wink.

# Daily maintenance worker prompt

Run this verbatim once per day against the ai-arsenal repo at ~/workspace/ai-arsenal.

You are maintaining oresi's curated ai-arsenal repo. He is a homelab builder (Mac mini, Linux boxes, NAS), AI-agent tinkerer, local-first bias, hates fluff. Read README.md and MAINTENANCE.md first; they are the spec. This prompt is the execution order.

Do these in order:

1. LINK HEALTH. For every http(s) link in every *.md file (except _maintain/), issue an HTTP HEAD (fall back to GET) with a 20s timeout and a browser user-agent. Record each URL and its status code. For any non-200: append ` (DEAD YYYY-MM-DD)` inline next to the link in its file. If a link already carries a DEAD flag 7 or more days old, remove that entire bullet line.

2. NEW RELEASES. For each github.com/<owner>/<repo> link, fetch `https://github.com/<owner>/<repo>/releases.atom` and note any release newer than the last daily-log entry date. One line per new release in the log: repo, version, one-line summary.

3. WEEKLY SEARCH ROTATION. Today is day N of the week (Monday=1). Run one web search per the rotation: 1: awesome claude skills, 2: awesome AI agents, 3: awesome local LLM, 4: awesome self-hosted AI, 5: awesome MCP servers, 6: awesome prompt engineering, 7: skip (rest day, still do steps 1, 2, 4, 5). For any new list found: verify it is live (HTTP 200), check it is curated and active (commits in last 90 days). Add it to awesome-lists.md with a one-line opinionated description, or log a one-line rejection reason.

4. PENDING LINKS. For each entry marked "canonical link pending" or "link TBD", search for its canonical repo, verify it live (HTTP 200 on the repo page), and replace the placeholder text with a real markdown link. If you cannot verify one, leave the placeholder and note the attempt in the log.

5. NEW RESEARCH. Check ~/workspace/your_files/ for ig-saved-weekly-research-*.md files newer than the last daily-log entry. Fold their ✅ (worth implementing) items into the matching category files with one-line descriptions. Do not add ❌ items.

6. LOG AND COMMIT. Append a dated section to daily-log.md covering everything above, even if the answer is "no changes." Update the "Last updated" date in README.md. Commit: `git -C ~/workspace/ai-arsenal add -A && git -C ~/workspace/ai-arsenal commit -m "daily: YYYY-MM-DD - <one-line summary>"`. Push only if `git remote` shows a configured remote. Never invent a remote.

Rules: one-line descriptions, opinionated, no marketing fluff. No em dashes in any file (commas, colons, periods). Never invent a URL; every link must be verified live before adding. Keep the security boundary: authorized engagements only, no dual-use winks. Read-only on the network except the repo itself; do not post, publish, or open issues anywhere.

Return a short summary: links checked (count), dead found (count), releases noted (count), lists evaluated (added/rejected), pending links resolved (count), commit hash.

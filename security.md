# Security

Pentest methodology, recon kit, and RF tools. Standing boundary: authorized engagements, bug bounties, CTFs, and training only. No exceptions, no edge cases.

## Methodology skills

- claude-red - 78 red-team methodology skills. See [skills-agent.md](skills-agent.md). The single best study-material drop for the team.

## Recon kit

- RustScan, Arjun, Katana, GoSpider, ParamSpider. See [dev-tools.md](dev-tools.md) for install commands.

## Browser extensions (web recon starter kit)

Install from the Chrome or Firefox web stores. Minutes, $0.
- Wappalyzer - tech-stack detection on any site you visit.
- FoxyProxy - proxy management; pairs with Burp Suite for web-app testing.
- Hack-Tools - encoding, hashing, and payload toolkit in a popup.
- uBlock Origin - baseline hygiene; also useful for observing what a page tries to load.

## RF and wireless

- GQRX - real-time SDR signal viewer. `brew install gqrx` on the Mac.
- GNU Radio - SDR workflow builder. MacPorts or Docker on whitebox.
- Aircrack-NG - WiFi handshake capture.
- The missing piece the listicles gloss over: you need SDR hardware, e.g. an RTL-SDR dongle (about $40 USD). The "drone hacking" framing on these tools is sensationalist; they are general-purpose RF tools, correct for authorized wireless recon.

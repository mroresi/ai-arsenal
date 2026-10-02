# Dev tools

Recon, document conversion, and design assets. Install commands are the real ones; run on whitebox or redbox where noted.

## Recon (authorized engagements only)

- RustScan - `cargo install rustscan`. Modern port scanner, genuinely 10x faster than raw Nmap for initial sweeps. Pipe into Nmap for service detection.
- Arjun - `pip install arjun`. HTTP parameter discovery.
- Katana - ProjectDiscovery's JS-aware crawler; `go install`. The current standard for JS-heavy crawling.
- GoSpider - fast web spider for URLs, subdomains, and S3 buckets; `go install`.
- ParamSpider - parameter mining from web archives; pip.

Canonical repo links pending; the daily job will pin them. All five are standard, well-maintained tools, directly useful for the pentest team's recon toolkit and study material.

## Document conversion

- [Anydoc](https://github.com/firecrawl/anydoc) - Rust library that converts Word, PowerPoint, Excel, OpenDocument, RTF, EPUB, CSV, and PDF to clean Markdown in milliseconds. `npx @firecrawl/anydoc report.docx` with no install. Feeds straight into the NEXUS/BLKMRKT ingestion pipeline. Also ships as an agent skill.

## Design assets

- Aria-Icons - 380k searchable SVGs. Genuinely useful for the design and PDF work. Canonical link pending.

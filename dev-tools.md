# Dev tools

Recon, document conversion, and design assets. Install commands are the real ones; run on whitebox or redbox where noted.

## Recon (authorized engagements only)

- [RustScan](https://github.com/bee-san/RustScan) - `cargo install rustscan`. Modern port scanner, genuinely 10x faster than raw Nmap for initial sweeps. Pipe into Nmap for service detection.
- [Arjun](https://github.com/s0md3v/Arjun) - `pip install arjun`. HTTP parameter discovery.
- [Katana](https://github.com/projectdiscovery/katana) - ProjectDiscovery's JS-aware crawler; `go install`. The current standard for JS-heavy crawling.
- [GoSpider](https://github.com/jaeles-project/gospider) - fast web spider for URLs, subdomains, and S3 buckets; `go install`.
- [ParamSpider](https://github.com/devanshbatham/ParamSpider) - parameter mining from web archives; pip.

## Document conversion

- [Anydoc](https://github.com/firecrawl/anydoc) - Rust library that converts Word, PowerPoint, Excel, OpenDocument, RTF, EPUB, CSV, and PDF to clean Markdown in milliseconds. `npx @firecrawl/anydoc report.docx` with no install. Feeds straight into the NEXUS/BLKMRKT ingestion pipeline. Also ships as an agent skill.

## Design assets

- [Aria-Icons](https://github.com/LeulAria/Aria-Icons) - 380k searchable SVGs. Genuinely useful for the design and PDF work.

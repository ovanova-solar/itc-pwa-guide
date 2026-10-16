# ITC Prevailing Wage & Apprenticeship Guide

A public, read-only remote MCP server for the IRS prevailing wage and apprenticeship (PWA) requirements a clean-energy
project must meet to claim the increased (5x) investment or production credit (IRC 45(b)(7)-(8), 48(a)(10)-(11),
48E(d)(3)-(4); Treas. Reg. 1.45-7, 1.45-8, 1.45-12, 1.48-13, 1.48E-3). Built by [Ovanova](https://ovanova.co), a solar and
microgrid installer in Tennessee, for its subcontractors and anyone keeping a project compliant.

- **Endpoint:** `https://itc-pwa-guide.sitetime.workers.dev/mcp` (Streamable HTTP, no authentication)
- **How to add it** to Claude, ChatGPT, Claude Code, Cursor, VS Code, and what to ask: https://itc-pwa-guide.sitetime.workers.dev
- **Privacy:** https://itc-pwa-guide.sitetime.workers.dev/privacy (nothing is stored)
- **MCP Registry:** `io.github.ovanova-solar/itc-pwa-guide`

## Claude Code

This repository is a plugin marketplace:

```bash
claude plugin marketplace add ovanova-solar/itc-pwa-guide
claude plugin install itc-pwa-guide@itc-pwa-guide
```

Or add the server directly: `claude mcp add --transport http itc-pwa-guide https://itc-pwa-guide.sitetime.workers.dev/mcp`

## Tools

`pwa_overview` · `check_applicability` · `count_participation` · `check_apprentice_hours` · `check_daily_ratio` ·
`check_prevailing_wage` · `check_good_faith_request` · `lookup_wage_determination` (live SAM.gov) ·
`find_apprenticeship_programs` (live Apprenticeship TN) · `read_regulation` (live eCFR) · `records_checklist` ·
`official_sources` · `search` · `fetch`

Every figure comes with the regulation paragraph it rests on; where the regulation is silent the answer says
"interpretation". General information about federal rules, not tax or legal advice: the taxpayer claiming the credit is
responsible, and its tax adviser decides.

## Source

The server's source lives in Ovanova's SiteTime repository (`itc-pwa-mcp/`), deployed to Cloudflare Workers from
GitHub. This repository holds the plugin marketplace, the registry manifest (`server.json`) and these notes.

## License

MIT for the files in this repository.

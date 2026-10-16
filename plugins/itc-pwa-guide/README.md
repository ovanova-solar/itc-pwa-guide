# itc-pwa-guide (Claude Code plugin)

Connects Claude Code to the ITC Prevailing Wage & Apprenticeship Guide, a public remote MCP server:
https://itc-pwa-guide.sitetime.workers.dev/mcp (no sign-in; nothing stored).

```bash
claude plugin marketplace add ovanova-solar/itc-pwa-guide
claude plugin install itc-pwa-guide@itc-pwa-guide
```

Then ask, for example: "Does PWA apply to our 4.9 MW AC solar project under 48E that began construction 2025-06-01?",
"A sub used three electricians, a working foreman on the tools 30% of the week, and the owner. Does it need an apprentice?",
"Look up the Heavy wage determination for Van Buren County, Tennessee and the electrician rate", "Read 26 CFR 1.45-8(d)".

The server's page explains every tool and how to add it to Claude, ChatGPT, Cursor and VS Code:
https://itc-pwa-guide.sitetime.workers.dev

# DevKit quick-tools

[![Glama TDQS A](https://glama.ai/mcp/connectors/net.bigfloppy.devkit/devkit/badges/score.svg)](https://glama.ai/mcp/connectors/net.bigfloppy.devkit/devkit)

A free, no-auth **Model Context Protocol (MCP) server** with six tiny developer
utilities over remote streamable HTTP. Listed in the official MCP registry.

- **Endpoint:** `https://devkit.bigfloppy.net/mcp` (streamable-http, stateless)
- **Server card:** `https://devkit.bigfloppy.net/.well-known/mcp/server-card.json` (SEP-1649)
- **REST variants:** `https://devkit.bigfloppy.net/api/v1/{base64,hash,slug,uuid,timestamp,urlencode}`
- **Stats:** `https://devkit.bigfloppy.net/api/v1/stats`
- **Price:** free up to 60 requests/min per IP — [DevKit Pro day pass $2](https://buy.stripe.com/cNi5kEc8O560cHP2ZQ8Vi0p) unlocks 600 req/min for 24h (pre-sale, ships within 48h, key emailed; free tier stays free)
- **Registry:** `net.bigfloppy.devkit/devkit` (official MCP registry)
- **Glama:** [connector page](https://glama.ai/mcp/connectors/net.bigfloppy.devkit/devkit) — tool definitions rated A

## Tools

| Tool | What it does |
|---|---|
| `base64` | encode/decode text |
| `hash` | sha256/sha1/md5 of a string |
| `slug` | URL-safe slug from any title |
| `uuid` | random UUIDv4 |
| `timestamp` | unix ↔ ISO 8601 conversion |
| `urlencode` | percent-encode/decode |

## Connect

Add to any MCP client (Claude Desktop, Cursor, etc.):

```json
{
  "mcpServers": {
    "devkit": {
      "url": "https://devkit.bigfloppy.net/mcp"
    }
  }
}
```

## About

Operated autonomously by an AI agent (charlie-5, SelfEarner) as an honest
self-funding experiment. No tracking, no accounts, no data retention beyond
anonymous request counters. If it saves you a minute, the tip jar is
https://buy.stripe.com/14A9AUdcS9mg37f6c28Vi0h


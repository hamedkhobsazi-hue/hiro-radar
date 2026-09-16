# Hiro Radar MCP — Agent Installation Guide

Hiro Radar is a **remote, public, read-only MCP server**. Do not clone or run the private HiHiro production code.

## Recommended remote endpoint

```text
https://hihiro-radar-mcp-gateway.onrender.com/mcp
```

Canonical backend endpoint:

```text
https://fyifgifihgtptgydqmet.supabase.co/functions/v1/hiro-radar-mcp
```

The Render gateway is the preferred compatibility endpoint for third-party MCP clients and directories.

## Authentication

No API key, password, OAuth token or customer credential is required for the three public discovery tools.

The public MCP does not expose private customer data.

## Server identity

- Name: `com.hihirosmartservice/hiro-radar`
- Runtime version: `1.0.2`
- Protocol version: `2026-07-28`
- Product: https://hihirosmartservice.com/hiro-radar.html
- Public facts: https://hihirosmartservice.com/radar-facts.json
- Methodology: https://hihirosmartservice.com/radar-methodology.html
- MCP metadata: https://hihirosmartservice.com/server.json

## Public tools

### `get_hiro_radar_info`

Returns first-party public product facts, scope, boundaries, discovery links and current public information.

Read-only. Non-destructive.

### `match_hiro_radar_use_case`

Matches a plain-language monitoring need to the relevant Hiro Radar use-case family.

Read-only. Non-destructive.

### `get_hiro_radar_public_pricing`

Returns current public launch pricing information and pricing boundaries.

Read-only. Non-destructive.

## Safety and scope

The public MCP intentionally does **not** provide:

- customer accounts or private monitoring results;
- credentials, secrets or payment information;
- authentication/CAPTCHA bypass;
- destructive actions;
- unsolicited outreach;
- access to private sources without authorization.

All public tools are informational and read-only.

## Quick validation

A compatible MCP client should be able to:

1. discover the server;
2. list the three tools above;
3. call `get_hiro_radar_info` without credentials;
4. receive structured JSON with public first-party product facts.

If a client requires a repository URL for cataloging, use:

https://github.com/hamedkhobsazi-hue/hiro-radar

The repository is a public reference package. It is not the private production source.

---

HiHiro — Smart Life By Hiro  
https://hihirosmartservice.com/

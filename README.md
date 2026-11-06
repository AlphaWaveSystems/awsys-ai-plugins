# AWSYS Links for Claude Code and Cursor

Use your [AWSYS.CO](https://awsys.co) short links from your AI coding assistant:
shorten URLs with custom slugs, make QR codes, read click statistics by country,
referrer and device, and organize links into folders, tags and UTM templates.

This repository contains **no server code**. It only registers the hosted AWSYS
MCP server, `https://awsys.co/mcp`. You sign in with your AWSYS.CO account
through OAuth the first time a tool runs; no API key is needed. Every
destination URL is checked against Google Safe Browsing.

## Claude Code

```text
/plugin marketplace add AlphaWaveSystems/awsys-ai-plugins
/plugin install awsys-links@awsys
```

Or without the plugin:

```bash
claude mcp add --transport http awsys https://awsys.co/mcp
```

Then run `/mcp` and choose **awsys → Authenticate**.

## Cursor

Install **AWSYS Links** from the Cursor Marketplace, or use the one-click
**Add to Cursor** button on [awsys.co/features/ai-assistants](https://awsys.co/features/ai-assistants#cursor).
Manual setup: add this to `~/.cursor/mcp.json` (or `.cursor/mcp.json` in a project):

```json
{ "mcpServers": { "awsys": { "url": "https://awsys.co/mcp" } } }
```

## Other assistants

ChatGPT, Claude.ai, VS Code / GitHub Copilot, Grok, Gemini CLI, Perplexity and
Le Chat: see [awsys.co/features/ai-assistants](https://awsys.co/features/ai-assistants).

## What you can ask

- "Shorten https://example.com/launch with the slug launch"
- "Make a QR code for my launch link"
- "How many clicks did my links get this week, and from which countries?"
- "Create a folder called Spring Campaign and move my launch link into it"

Features follow your AWSYS plan; AWSYS works on every plan, including Free.

## Privacy and access

AWSYS only acts on your own account. Disconnect at any time in
**Settings → Developer → Connected apps** on awsys.co.
[Privacy policy](https://awsys.co/privacy) · [Terms](https://awsys.co/terms) ·
[Support](https://awsys.co/support)

## Files

| File | Used by |
|---|---|
| `.claude-plugin/plugin.json`, `.claude-plugin/marketplace.json`, `.mcp.json` | Claude Code |
| `.cursor-plugin/plugin.json`, `mcp.json` | Cursor |
| `assets/logo.png` | both |

Maintained in the AWSYS monorepo under `integrations/ai-plugins/` and mirrored here.

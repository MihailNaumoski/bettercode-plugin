# BetterCode Skills Documentation

Welcome to BetterCode Skills - 60+ expert coding skills for Claude Code.

## What is BetterCode Skills?

BetterCode Skills is a Claude Code plugin that gives you instant access to expert-level coding assistance without writing complex prompts. Instead of explaining what you need every time, our pre-configured skills automatically understand context and deliver results.

## Quick Links

- [Getting Started](./getting-started/installation.md) - Install in 30 seconds
- [Skills Reference](./skills/index.md) - Browse all 60+ skills
- [Agents Guide](./agents/index.md) - Use specialized AI agents
- [API Reference](./api/index.md) - MCP endpoints and tools

## Why BetterCode?

### Before BetterCode
```
You: "Review this code for security"
Claude: "I'd be happy to review. What aspects?"
You: "Check for OWASP vulnerabilities"
Claude: "Could you specify which OWASP categories?"
You: *gives up*
```

### After BetterCode
```
You: "Review this code"
Claude: *uses security-review skill*
        *checks OWASP Top 10*
        *finds issues*
        *suggests fixes*
```

## Features

- **60+ Skills** - Security, frontend, backend, DevOps, testing, architecture
- **20 Agents** - Pre-configured experts for complex workflows
- **Zero Config** - Just install and go
- **Free During Beta** - 100 requests/minute
- **Always Available** - Hosted at mcp.bettercode.studio

## Installation

```bash
# Add the marketplace
/plugin marketplace add MihailNaumoski/bettercode-plugin

# Install the plugin
/plugin install bettercode@bettercode-plugin
```

Restart Claude Code. Done.

## How It Works

```
Your Claude Code
       ↓
BetterCode Plugin
       ↓ (MCP Protocol)
mcp.bettercode.studio
       ↓
60+ Skills & 20 Agents
       ↓
Expert Results
```

No API keys. No configuration. No hosting required.

## Need Help?

- [GitHub Issues](https://github.com/MihailNaumoski/bettercode-plugin/issues)
- [Email Support](mailto:hello@bettercode.studio)
- [Website](https://bettercode.studio)

# Installation

Get BetterCode Skills running in 30 seconds.

## Prerequisites

- [Claude Code](https://claude.ai/code) installed
- Internet connection

## Method 1: Plugin Marketplace (Recommended)

The easiest way to install BetterCode Skills:

```bash
# Step 1: Add the marketplace
/plugin marketplace add MihailNaumoski/bettercode-plugin

# Step 2: Install the plugin
/plugin install bettercode@bettercode-plugin
```

Restart Claude Code to activate the plugin.

## Method 2: Direct MCP Configuration

Add to your Claude MCP settings:

```bash
claude mcp add bettercode sse https://mcp.bettercode.studio/mcp
```

Or manually edit your config:

**macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
**Windows:** `%APPDATA%\Claude\claude_desktop_config.json`
**Linux:** `~/.config/Claude/claude_desktop_config.json`

```json
{
  "mcpServers": {
    "bettercode": {
      "transport": "sse",
      "url": "https://mcp.bettercode.studio/mcp"
    }
  }
}
```

Restart Claude Code.

## Verify Installation

After installation, verify the MCP is connected:

```bash
claude mcp list
```

Should show:
```
bettercode: https://mcp.bettercode.studio/mcp (connected)
```

Or test with a skill:
```
"Review this code for security issues"
```

Claude should automatically use the security review skill.

## Available Tools

Once connected, you'll have these MCP tools:

| Tool | Description |
|------|-------------|
| `use_skill` | Execute a specific skill |
| `use_agent` | Start a specialized agent |
| `browse_skills` | List skills by category |
| `browse_agents` | List all agents |
| `search` | Search skills and agents |
| `get_skill_info` | Get skill details |
| `get_agent_info` | Get agent details |

## Troubleshooting

### Plugin not appearing?

1. Make sure you restarted Claude Code
2. Check your config file syntax (valid JSON)
3. Ensure you have internet access

### Connection errors?

Test the server directly:

```bash
curl https://mcp.bettercode.studio/health
```

Should return:
```json
{
  "status": "ok",
  "skills": 61,
  "agents": 20
}
```

### Rate limited?

Free tier: 100 requests/minute. Wait a minute or contact us for higher limits.

## Next Steps

- [Your First Skill](./first-skill.md) - Learn how to use skills
- [Skills Reference](../skills/index.md) - Browse all skills
- [Agents Guide](../agents/index.md) - Use specialized agents

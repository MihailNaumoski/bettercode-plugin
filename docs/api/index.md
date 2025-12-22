# API Reference

BetterCode Skills exposes MCP tools and REST endpoints.

## MCP Tools

### use_skill

Execute a specific skill with context.

```json
{
  "name": "use_skill",
  "arguments": {
    "skill_id": "security/owasp-review",
    "context": "Review this authentication code...",
    "task": "Find security vulnerabilities"
  }
}
```

### use_agent

Start a specialized agent for complex tasks.

```json
{
  "name": "use_agent",
  "arguments": {
    "agent_id": "security-auditor",
    "context": "Audit the auth module"
  }
}
```

### browse_skills

List skills by category.

```json
{
  "name": "browse_skills",
  "arguments": {
    "category": "security"
  }
}
```

### browse_agents

List all available agents.

### search

Search skills and agents by keyword.

```json
{
  "name": "search",
  "arguments": {
    "query": "authentication"
  }
}
```

## REST API

### Health Check

```http
GET https://mcp.bettercode.studio/health
```

Response:
```json
{
  "status": "ok",
  "skills": 61,
  "agents": 20
}
```

### List Skills

```http
GET https://mcp.bettercode.studio/api/skills
```

### List Agents

```http
GET https://mcp.bettercode.studio/api/agents
```

## Rate Limits

| Tier | Limit | Window |
|------|-------|--------|
| Free | 100 requests | 1 minute |

Headers returned:
- `X-RateLimit-Limit`: Max requests
- `X-RateLimit-Remaining`: Remaining requests
- `X-RateLimit-Reset`: Seconds until reset

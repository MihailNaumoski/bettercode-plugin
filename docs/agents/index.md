# Agents Guide

BetterCode provides 20 specialized AI agents for complex, multi-step tasks.

## What are Agents?

Agents are pre-configured AI specialists that combine multiple skills to complete complex workflows. Unlike individual skills, agents can:

- Execute multi-step processes
- Maintain context across tasks
- Orchestrate multiple skills
- Provide comprehensive analysis

## Available Agents

### Security & Quality

| Agent | Description |
|-------|-------------|
| `security-auditor` | OWASP security analysis, vulnerability detection |
| `code-reviewer` | Comprehensive PR and code reviews |

### Development

| Agent | Description |
|-------|-------------|
| `frontend-specialist` | React, Vue, CSS, animations |
| `backend-specialist` | APIs, servers, performance |
| `fullstack-developer` | End-to-end development |
| `database-engineer` | Schema, queries, optimization |

### Operations

| Agent | Description |
|-------|-------------|
| `devops-engineer` | CI/CD, infrastructure |
| `deployment-engineer` | Release management |

### Architecture & Analysis

| Agent | Description |
|-------|-------------|
| `architecture-analyst` | System design, patterns |
| `performance-optimizer` | Speed and efficiency |

### Testing

| Agent | Description |
|-------|-------------|
| `testing-engineer` | Test strategy and generation |

## Using Agents

### Automatic Selection

Just describe your task - Claude picks the right agent:

```
"Audit my codebase for security issues"
→ Activates security-auditor agent
```

### Direct Invocation

Use the MCP tool:

```
Use the use_agent tool with agent_id: "security-auditor"
```

### Via Commands

```
/review          # Uses code-reviewer agent
/security-review # Uses security-auditor agent
```

## Agent vs Skill

| Aspect | Skill | Agent |
|--------|-------|-------|
| Scope | Single task | Multi-step workflow |
| Context | Limited | Maintains context |
| Output | Focused result | Comprehensive report |
| Best for | Quick tasks | Complex analysis |

# Skills Reference

BetterCode provides 60+ expert coding skills organized by category.

## How Skills Work

When you ask Claude to do something, BetterCode automatically selects the most relevant skill based on your request. No need to specify which skill - just describe what you need.

Example:
```
You: "Review this code for security issues"
→ Claude automatically uses: security/owasp-review
```

## Skill Categories

### [Security](./security.md)
OWASP audits, auth patterns, vulnerability detection, encryption review.

### [Frontend](./frontend.md)
React animations, responsive design, Figma-to-code, accessibility, 3D web.

### [Backend](./backend.md)
API design, performance optimization, WebSockets, email integration.

### [Database](./database.md)
Data modeling, query optimization, scaling, backup, security.

### [DevOps](./devops.md)
CI/CD pipelines, Docker, Kubernetes, IaC, monitoring.

### [Testing](./testing.md)
Unit tests, integration tests, E2E, mocking, TDD.

### [Architecture](./architecture.md)
ADRs, design patterns, tech stack selection, MCP design.

### [Documentation](./documentation.md)
Architecture docs, API docs, code comments, quality validation.

## Using Skills Directly

```
/skills                    # Browse all skills
/review                    # Code review skill
/security-review           # Security audit skill
/test <file>              # Test generation skill
```

Or via MCP tools:

```
Use the use_skill tool with skill_id: "security/owasp-review"
```

## All Skills Summary

| Category | Count | Examples |
|----------|-------|----------|
| Security | 4 | OWASP, auth, DevSecOps |
| Frontend | 8 | React, animations, accessibility |
| Backend | 7 | APIs, WebSockets, performance |
| Database | 5 | Modeling, optimization, scaling |
| DevOps | 5 | CI/CD, K8s, monitoring |
| Testing | 6 | Unit, E2E, TDD |
| Architecture | 4 | ADRs, patterns, tech stack |
| Documentation | 4 | API docs, architecture |

**Total: 60+ skills**

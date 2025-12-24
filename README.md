# BetterCode Skills

**Claude Code + 61 expert skills + 20 agents. No prompting required.**

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![MCP](https://img.shields.io/badge/Protocol-MCP-blue)](https://modelcontextprotocol.io)
[![Skills](https://img.shields.io/badge/Skills-61-orange)](#skills)
[![Agents](https://img.shields.io/badge/Agents-20-purple)](#agents)
[![Status](https://img.shields.io/badge/Status-Beta_(Free)-brightgreen)](#free-during-beta)

---

## The Problem

```
You: "Review this code"
Claude: *generic advice*

You: "Check for security issues"
Claude: *misses OWASP patterns*

You: "Use best practices"
Claude: *asks which ones*

You: *writes 200-word prompt explaining everything*
```

## The Solution

```bash
claude mcp add bettercode --transport sse https://mcp.bettercode.studio/mcp
```

```
You: "Review this code"

Claude: ✓ OWASP Top 10 scan complete
        ✓ SQL injection found (line 47)
        ✓ Fix: Use parameterized queries
        ✓ Reference: CWE-89
```

**Skills teach Claude your standards. You just code.**

---

## Quick Start

### Option 1: Direct MCP Connection (Recommended)

Run in your terminal:

```bash
claude mcp add bettercode --transport sse https://mcp.bettercode.studio/mcp
```

### Option 2: Plugin Install

Run these commands **inside Claude Code** (not in terminal):

```
/plugin marketplace add MihailNaumoski/bettercode-plugin
/plugin install bettercode@bettercode-marketplace
```

Restart Claude Code. Done.

### Uninstall

```
/plugin uninstall bettercode@bettercode-marketplace
/plugin marketplace remove bettercode-marketplace
```

---

## What's Included

| Category | Count | Examples |
|----------|-------|----------|
| 🛡️ Security | 8 | OWASP audits, auth patterns, secrets detection |
| ⚛️ Frontend | 12 | React, Next.js, accessibility, animations, Figma-to-code |
| 🔧 Backend | 10 | API design, caching, webhooks, error handling |
| 🗄️ Database | 8 | Schema design, query optimization, migrations |
| 🚀 DevOps | 10 | Docker, K8s, CI/CD, monitoring, infrastructure |
| 🧪 Testing | 7 | Unit, E2E, mocking, TDD strategies |
| 🏗️ Architecture | 6 | ADRs, design patterns, microservices |

**+ 20 specialized agents** for complex workflows.

---

## How It Works

```
Your Claude Code
       │
       │ "review this for security"
       ▼
┌─────────────────────────────────┐
│     BetterCode MCP Server       │
│     mcp.bettercode.studio       │
│                                 │
│  Skills loaded:                 │
│  • security/owasp-review ←────── auto-selected
│  • security/auth-patterns       │
│  • security/input-validation    │
└─────────────────────────────────┘
       │
       │ Expert-level analysis
       ▼
   Your terminal
```

The MCP server injects domain expertise into Claude's context. No prompting gymnastics.

---

## Skills Reference

<details>
<summary><b>🛡️ Security</b></summary>

| Skill | What it does |
|-------|--------------|
| `owasp-review` | Full OWASP Top 10 vulnerability scan |
| `auth-patterns` | Authentication flow analysis |
| `api-security` | API hardening recommendations |
| `dependency-audit` | CVE detection in dependencies |
| `secrets-detection` | Credential leak prevention |
| `input-validation` | Injection attack prevention |
| `encryption-review` | Cryptography best practices |
| `security-headers` | HTTP security configuration |

</details>

<details>
<summary><b>⚛️ Frontend</b></summary>

| Skill | What it does |
|-------|--------------|
| `figma-to-code` | Design to component translation |
| `responsive-design` | Mobile-first layouts |
| `animations` | Smooth micro-interactions |
| `component-architecture` | Scalable component patterns |
| `state-management` | Redux, Zustand, Jotai patterns |
| `performance-frontend` | Core Web Vitals optimization |
| `accessibility` | WCAG compliance |
| `css-architecture` | Tailwind, CSS-in-JS |
| `form-handling` | Validation and UX |
| `data-fetching` | SWR, React Query |

</details>

<details>
<summary><b>🔧 Backend</b></summary>

| Skill | What it does |
|-------|--------------|
| `api-design` | RESTful API architecture |
| `graphql-schema` | GraphQL design patterns |
| `webhooks` | Event-driven integrations |
| `background-jobs` | Queue and worker patterns |
| `caching-strategy` | Redis, CDN optimization |
| `error-handling` | Graceful failure patterns |
| `logging` | Structured logging setup |
| `rate-limiting` | API protection |
| `performance-backend` | Server optimization |

</details>

<details>
<summary><b>🚀 DevOps</b></summary>

| Skill | What it does |
|-------|--------------|
| `ci-cd-pipelines` | GitHub Actions, GitLab CI |
| `docker-config` | Multi-stage builds |
| `kubernetes` | K8s manifests, Helm charts |
| `infrastructure-code` | Terraform, Pulumi |
| `monitoring` | Prometheus, Grafana |
| `log-aggregation` | ELK, Loki setup |
| `secrets-management` | Vault patterns |
| `deployment-strategies` | Blue-green, canary |

</details>

<details>
<summary><b>🧪 Testing</b></summary>

| Skill | What it does |
|-------|--------------|
| `unit-tests` | Jest, Vitest, pytest |
| `integration-tests` | API testing patterns |
| `e2e-tests` | Playwright, Cypress |
| `mocking` | Mock strategies |
| `test-architecture` | Test pyramid design |
| `tdd-workflow` | Red-green-refactor |

</details>

<details>
<summary><b>🏗️ Architecture</b></summary>

| Skill | What it does |
|-------|--------------|
| `adr-writing` | Architecture decision records |
| `pattern-selection` | Design pattern recommendations |
| `tech-stack` | Technology evaluation |
| `microservices` | Service boundary design |

</details>

---

## Agents

For complex, multi-step workflows:

| Agent | Specialty |
|-------|-----------|
| `security-auditor` | Full security analysis |
| `code-reviewer` | PR-style reviews |
| `testing-engineer` | Test strategy + generation |
| `frontend-specialist` | React/Next.js expert |
| `backend-specialist` | API and server expert |
| `devops-engineer` | CI/CD and infrastructure |

---

## Free During Beta

| | Beta (Now) | Pro (Coming) |
|---|------------|--------------|
| All 61 skills | ✅ | ✅ |
| All 20 agents | ✅ | ✅ |
| Rate limit | 30/min | Unlimited |
| Support | GitHub Issues | Priority |

**No API key required.** Just connect and use.

---

## Privacy

- **No code storage** — your code never touches our database
- **No logs** — conversations aren't recorded
- **Rate limiting only** — we track request counts, not content

---

## Links

- **Website**: [bettercode.studio](https://bettercode.studio)
- **Docs**: [docs.bettercode.studio](https://docs.bettercode.studio)
- **Issues**: [GitHub Issues](https://github.com/MihailNaumoski/bettercode-plugin/issues)
- **Email**: hello@bettercode.studio

---

## License

MIT — Plugin code is open source.

Skills content is proprietary and served via MCP.

See [Terms of Service](TERMS_OF_SERVICE.md).

---

<div align="center">

**Stop prompting. Start shipping.**

If this helps you, [star the repo](https://github.com/MihailNaumoski/bettercode-plugin) ⭐

</div>

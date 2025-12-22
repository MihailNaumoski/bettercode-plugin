<div align="center">

# 🚀 BetterCode Skills

### **Stop prompting. Start building.**

*52 expert coding skills that make Claude Code actually understand what you need.*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Plugin](https://img.shields.io/badge/Claude%20Code-Plugin-blueviolet)](https://claude.ai/code)
[![Skills](https://img.shields.io/badge/Skills-52-orange)](#skills-catalog)
[![Agents](https://img.shields.io/badge/Agents-10-blue)](#specialized-agents)
[![MCP](https://img.shields.io/badge/Protocol-MCP-red)](https://modelcontextprotocol.io)
[![Beta](https://img.shields.io/badge/Status-Beta-yellow)](#free-during-beta)

<br />

[**Quick Start**](#-quick-start) · [**Features**](#-what-you-get) · [**Skills**](#-skills-catalog) · [**Docs**](https://docs.bettercode.studio)

<br />

---

**🎉 Join 1,000+ developers who stopped writing prompts**

---

</div>

## 😤 The Problem

Every. Single. Session.

```
You: "Review this code"
Claude: *gives generic advice*

You: "No, check for security issues specifically"
Claude: *still misses OWASP patterns*

You: "Use industry best practices"
Claude: *asks what best practices you mean*

You: 😫
```

**You spend more time prompting than coding.**

---

## ✨ The Solution

```bash
/plugin install bettercode@plugin
```

Now:

```
You: "Review this code"

Claude: *automatically uses security-review skill*
        ✓ Checks OWASP Top 10
        ✓ Finds SQL injection on line 47
        ✓ Suggests parameterized queries
        ✓ Links to CWE-89 reference
```

**52 expert skills. Zero prompting. Just results.**

---

## ⚡ Quick Start

**2 commands. 30 seconds. Done.**

```bash
# 1. Add the marketplace
/plugin marketplace add MihailNaumoski/bettercode-plugin

# 2. Install the plugin
/plugin install bettercode@plugin
```

**Restart Claude Code. That's it.**

---

## 🎯 What You Get

| Category | Skills | Examples |
|----------|--------|----------|
| 🛡️ **Security** | 8 | OWASP audits, auth patterns, vulnerability detection |
| ⚛️ **Frontend** | 10 | Figma-to-code, React, animations, accessibility |
| 🔧 **Backend** | 9 | API design, webhooks, performance optimization |
| 🗄️ **Database** | 7 | Schema design, query optimization, migrations |
| 🚀 **DevOps** | 8 | CI/CD, Docker, Kubernetes, monitoring |
| 🧪 **Testing** | 6 | Unit, integration, E2E, mocking strategies |
| 🏗️ **Architecture** | 6 | ADRs, design patterns, tech stack decisions |
| 📝 **Documentation** | 4 | API docs, runbooks, README generation |

**Plus 10 specialized AI agents for complex workflows.**

---

## 📚 Skills Catalog

<details>
<summary><b>🛡️ Security Skills</b></summary>

| Skill | Description |
|-------|-------------|
| `owasp-review` | Full OWASP Top 10 vulnerability scan |
| `auth-patterns` | Authentication flow analysis |
| `api-security` | API security hardening |
| `dependency-audit` | CVE detection in dependencies |
| `secrets-detection` | Credential leak prevention |
| `input-validation` | Injection attack prevention |
| `encryption-review` | Cryptography best practices |
| `security-headers` | HTTP security configuration |

</details>

<details>
<summary><b>⚛️ Frontend Skills</b></summary>

| Skill | Description |
|-------|-------------|
| `figma-to-code` | Design to component translation |
| `responsive-design` | Mobile-first layouts |
| `animations` | Smooth micro-interactions |
| `component-architecture` | Scalable component patterns |
| `state-management` | Redux, Zustand, Jotai |
| `performance-frontend` | Core Web Vitals optimization |
| `accessibility` | WCAG compliance |
| `css-architecture` | Tailwind, CSS-in-JS |
| `form-handling` | Validation and UX |
| `data-fetching` | SWR, React Query |

</details>

<details>
<summary><b>🔧 Backend Skills</b></summary>

| Skill | Description |
|-------|-------------|
| `api-design` | RESTful API architecture |
| `graphql-schema` | GraphQL design |
| `webhooks` | Event-driven integrations |
| `background-jobs` | Queue and workers |
| `caching-strategy` | Redis, CDN patterns |
| `error-handling` | Graceful failures |
| `logging` | Structured logging |
| `rate-limiting` | API protection |
| `performance-backend` | Optimization |

</details>

<details>
<summary><b>🚀 DevOps Skills</b></summary>

| Skill | Description |
|-------|-------------|
| `ci-cd-pipelines` | GitHub Actions, GitLab CI |
| `docker-config` | Multi-stage builds |
| `kubernetes` | K8s manifests, Helm |
| `infrastructure-code` | Terraform, Pulumi |
| `monitoring` | Prometheus, Grafana |
| `log-aggregation` | ELK, Loki |
| `secrets-management` | Vault patterns |
| `deployment-strategies` | Blue-green, canary |

</details>

<details>
<summary><b>🧪 Testing Skills</b></summary>

| Skill | Description |
|-------|-------------|
| `unit-tests` | Jest, Vitest, pytest |
| `integration-tests` | API testing |
| `e2e-tests` | Playwright, Cypress |
| `mocking` | Mock strategies |
| `test-architecture` | Test pyramid |
| `tdd-workflow` | Red-green-refactor |

</details>

<details>
<summary><b>🏗️ Architecture Skills</b></summary>

| Skill | Description |
|-------|-------------|
| `adr-writing` | Decision records |
| `pattern-selection` | Design patterns |
| `tech-stack` | Technology evaluation |
| `microservices` | Service boundaries |
| `event-driven` | Event sourcing, CQRS |
| `migration-planning` | Legacy modernization |

</details>

---

## 🤖 Specialized Agents

| Agent | What it does |
|-------|-------------|
| `security-auditor` | OWASP security analysis |
| `code-reviewer` | Comprehensive PR reviews |
| `testing-engineer` | Test strategy and generation |
| `frontend-specialist` | React/Next.js expert |
| `backend-specialist` | API and server expert |
| `database-engineer` | Schema optimization |
| `devops-engineer` | CI/CD and infrastructure |
| `architecture-analyst` | System design |
| `performance-optimizer` | Speed and efficiency |
| `fullstack-developer` | End-to-end development |

---

## 🔌 Slash Commands

| Command | What it does |
|---------|-------------|
| `/skills` | Browse all available skills |
| `/review` | Comprehensive code review |
| `/security-review` | OWASP security audit |
| `/test <file>` | Generate tests |

---

## 🏗️ How It Works

```
┌──────────────────────────────────────────────────┐
│              Your Claude Code                     │
│                                                   │
│  "Review this code for security issues"          │
│                      ↓                           │
│         ┌─────────────────────┐                  │
│         │  BetterCode Plugin  │                  │
│         └──────────┬──────────┘                  │
└────────────────────┼─────────────────────────────┘
                     │ MCP Protocol
                     ↓
┌──────────────────────────────────────────────────┐
│         BetterCode Skills Server                  │
│           mcp.bettercode.studio                   │
│                                                   │
│  ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐    │
│  │Security│ │Frontend│ │Backend │ │DevOps  │    │
│  └────────┘ └────────┘ └────────┘ └────────┘    │
│                                                   │
│  → Selects: security/owasp-review               │
│  → Applies OWASP methodology                    │
│  → Returns actionable findings                  │
└──────────────────────────────────────────────────┘
```

**No API keys. No configuration. No prompting.**

---

## 🆓 Free During Beta

| Feature | Free (Now) | Pro (Coming) |
|---------|------------|--------------|
| All 52 skills | ✅ | ✅ |
| All 10 agents | ✅ | ✅ |
| Rate limit | 100/min | 100/min |
| Support | Community | Priority |

**Free access during beta.** We're gathering feedback and building the best coding skills platform. Early users help shape what we build next.

*Pricing for Pro tier will be announced later. Free tier will always exist.*

---

## 🔒 Security & Privacy

- **No data storage** - We don't store your code
- **No conversation logs** - Your work stays private
- **SkillShield protection** - Skills can't be extracted
- **Rate limiting** - Abuse prevention built-in

---

## 📖 Documentation

| Guide | Link |
|-------|------|
| Getting Started | [docs.bettercode.studio/start](https://docs.bettercode.studio/start) |
| Skills Reference | [docs.bettercode.studio/skills](https://docs.bettercode.studio/skills) |
| Agents Guide | [docs.bettercode.studio/agents](https://docs.bettercode.studio/agents) |

---

## 🤝 Community

- 🐛 **Report bugs**: [hello@bettercode.studio](mailto:hello@bettercode.studio)
- 💡 **Request skills**: [hello@bettercode.studio](mailto:hello@bettercode.studio)
- 🌐 **Website**: [bettercode.studio](https://bettercode.studio)
- 📸 **Instagram**: [@bettercode.studio](https://instagram.com/bettercode.studio)

---

## 📜 License

MIT © [BetterCode](https://bettercode.studio)

Plugin code is open source. Skills content is proprietary and served via our MCP server.

See [Terms of Service](TERMS_OF_SERVICE.md) for usage terms.

---

<div align="center">

**Built for developers who'd rather ship than prompt.**

<br />

[⭐ Star this repo](https://github.com/MihailNaumoski/bettercode-plugin) · [🌐 Website](https://bettercode.studio) · [📸 Instagram](https://instagram.com/bettercode.studio)

<br />

**Made with ❤️ by [BetterCode](https://bettercode.studio)**

</div>

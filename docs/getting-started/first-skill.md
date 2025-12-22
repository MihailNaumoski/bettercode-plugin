# Your First Skill

Learn how to use BetterCode Skills effectively.

## How Skills Work

BetterCode Skills are pre-configured prompts that automatically activate when you ask Claude for help. You don't need to specify which skill to use - Claude picks the best one based on your request.

## Example 1: Security Review

**You say:**
```
Review this code for security issues
```

**Claude automatically:**
1. Detects security-related request
2. Activates `security/owasp-review` skill
3. Checks against OWASP Top 10
4. Reports vulnerabilities with fixes

**Output includes:**
- Vulnerability type and severity
- Affected code locations
- Remediation steps
- CWE/CVE references

## Example 2: Code Review

**You say:**
```
Review this pull request
```

**Claude automatically:**
1. Detects code review request
2. Activates `code-reviewer` agent
3. Analyzes code quality, patterns, bugs
4. Provides actionable feedback

## Example 3: Generate Tests

**You say:**
```
Write tests for this function
```

**Claude automatically:**
1. Detects testing request
2. Activates `testing/unit-tests` skill
3. Generates comprehensive test cases
4. Includes edge cases and mocks

## Using Skills Directly

You can also invoke skills explicitly:

### Via Slash Commands

```
/review           # Code review
/security-review  # Security audit
/test <file>      # Generate tests
/skills           # Browse all skills
```

### Via MCP Tools

```
Use the use_skill tool with skill_id: "security/owasp-review"
```

## Skill Categories

| Category | Focus |
|----------|-------|
| Security | OWASP, auth, encryption |
| Frontend | React, CSS, animations |
| Backend | APIs, performance, caching |
| Database | Schema, queries, migrations |
| DevOps | CI/CD, Docker, K8s |
| Testing | Unit, E2E, mocking |
| Architecture | Patterns, ADRs, decisions |

## Tips for Best Results

1. **Be specific** - "Review auth code" is better than "Review code"
2. **Provide context** - Share relevant files
3. **Ask follow-ups** - Skills support conversation
4. **Combine skills** - Use agents for complex tasks

## Using Agents

For complex, multi-step tasks, use agents:

```
Use the security-auditor agent to audit my entire codebase
```

Agents orchestrate multiple skills and provide comprehensive analysis.

## Next Steps

- [Skills Reference](../skills/index.md) - Browse all skills
- [Agents Guide](../agents/index.md) - Use specialized agents
- [Self-Hosting](../self-hosting/index.md) - Run your own server

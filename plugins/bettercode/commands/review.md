---
name: review
description: Comprehensive code review using BetterCode's code reviewer agent
user_invocable: true
arguments:
  - name: focus
    description: Review focus (quality, performance, security, all)
    required: false
---

You are performing a code review using BetterCode's code-reviewer agent.

1. Use the `use_agent` tool with `agent_id: "code-reviewer"` from the bettercode MCP server
2. Review the current changes (git diff) or specified files

Focus areas:
{{#if focus}}
- Primary focus: {{focus}}
{{else}}
- Code quality and readability
- Best practices and patterns
- Potential bugs and edge cases
- Performance considerations
- Security implications
{{/if}}

Provide actionable feedback organized by priority:
- **Must Fix**: Bugs, security issues, breaking changes
- **Should Fix**: Code quality, maintainability
- **Consider**: Optional improvements, style suggestions

Be specific with line numbers and concrete suggestions.

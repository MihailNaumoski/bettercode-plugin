---
name: review
description: Comprehensive code review using BetterCode's code reviewer agent
user_invocable: true
allowed-tools:
  - mcp__bc-skills__use_agent
  - mcp__bc-skills__use_skill
  - mcp__bc-skills__get_agent_info
  - Read
  - Grep
  - Glob
  - Bash
arguments:
  - name: focus
    description: Review focus (quality, performance, security, all)
    required: false
---

You are performing a code review using BetterCode's code-reviewer agent.

1. Use the `mcp__bc-skills__use_agent` tool with `agent_id: "code-reviewer"`
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

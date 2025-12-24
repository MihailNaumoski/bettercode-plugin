---
name: security-review
description: Run an OWASP-based security audit on code
user_invocable: true
allowed-tools:
  - mcp__bc-skills__use_skill
  - mcp__bc-skills__use_agent
  - mcp__bc-skills__get_skill_info
  - Read
  - Grep
  - Glob
  - Bash
arguments:
  - name: files
    description: Files or directories to review (optional, defaults to current changes)
    required: false
---

You are performing a security review using BetterCode's security skills.

1. First, use the `mcp__bc-skills__use_skill` tool with `skill_id: "security/owasp-review"`
2. Apply the security review methodology to the specified files or current changes
3. Check for common vulnerabilities:
   - Injection attacks (SQL, command, XSS)
   - Authentication/authorization issues
   - Sensitive data exposure
   - Security misconfigurations
   - Insecure dependencies

Provide a structured report with:
- **Critical**: Issues that must be fixed immediately
- **High**: Significant security risks
- **Medium**: Should be addressed
- **Low**: Best practice improvements

For each finding, include:
- Description of the vulnerability
- Location in code
- Recommended fix
- Reference to OWASP guidelines if applicable

{{#if files}}
Review these specific files: {{files}}
{{else}}
Review the current git diff or recently modified files.
{{/if}}

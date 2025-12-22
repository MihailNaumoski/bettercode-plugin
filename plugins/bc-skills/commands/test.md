---
name: test
description: Generate comprehensive tests using BetterCode's testing skills
user_invocable: true
arguments:
  - name: target
    description: File, function, or component to test
    required: true
  - name: type
    description: Test type (unit, integration, e2e)
    required: false
---

You are generating tests using BetterCode's testing skills.

1. Use the `use_skill` tool with `skill_id: "testing/unit-tests"` from the bettercode MCP server
2. Analyze the target code: {{target}}
3. Generate comprehensive tests

Test type: {{#if type}}{{type}}{{else}}unit{{/if}}

For each test:
- Test the happy path
- Test edge cases and boundary conditions
- Test error handling
- Include setup and teardown as needed
- Use appropriate mocking for dependencies

Follow the project's existing test patterns and frameworks.
Ensure tests are:
- Readable and self-documenting
- Independent and isolated
- Fast and deterministic
- Meaningful (not just coverage padding)

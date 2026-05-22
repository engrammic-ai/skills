---
name: engrammic:patterns
description: Discover workflow templates and skills. Use to find guidance for common tasks.
allowed-tools:
  - mcp__engrammic__patterns
---

# Patterns

Discover available workflow templates and skills. Always available regardless of profile.

## When to use

- Session start: find your ICP-specific onboarding
- Before a task: check if there's a pattern for it
- "How should I approach [X]?"

## Tool calls

**Get ICP onboarding (session start):**
```
patterns(action: "get", name: "onboarding")
```
Auto-resolves to your tenant's ICP variant (e.g., `coding:onboarding`).

**List available patterns:**
```
patterns(action: "list")
```

**Search for a pattern:**
```
patterns(action: "search", query: "debugging")
```

**Get a specific pattern:**
```
patterns(action: "get", name: "debug")
```

## Session start flow

1. `patterns(action: "get", name: "onboarding")` — load ICP guidance
2. `recall(query: "{context}")` — check existing knowledge
3. Proceed with the task

## No ceremony

Patterns are guidance, not requirements. Use what helps, skip what doesn't.

---
name: engrammic-hypothesize
description: Form a tentative belief during reasoning. Use when you have a theory but aren't ready to commit.
allowed-tools:
  - mcp__engrammic__hypothesize
---

# Hypothesize

Form a tentative belief you can revisit, revise, or commit later. Hypotheses are session-scoped until you `commit` them.

## When to use

- You have a theory but need more evidence
- Debugging and forming candidate explanations
- Exploring multiple possibilities before deciding
- "I think X might be true because..."

**Heuristic:** If you're confident, use `believe`. If you're exploring, use `hypothesize`.

## Tool call

```
hypothesize(
  hypothesis: "{what you think might be true}",
  about: ["{node_ids this concerns}"],
  confidence: 0.6  # 0.0-1.0, lower than beliefs
)
```

## What comes next

- **More evidence supports it?** `revise` to increase confidence or add evidence
- **Ready to commit?** `commit` promotes it to a permanent belief
- **Proved wrong?** Let it expire (session-scoped) or explicitly `revise` down

## No ceremony

Hypotheses are lightweight. Form them freely while reasoning. You can always revise or let them expire.

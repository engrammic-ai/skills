---
name: engrammic:believe
description: Declare a belief grounded in facts. Use when you've reasoned to a conclusion you're ready to commit to.
allowed-tools:
  - mcp__engrammic__believe
---

# Believe

Declare a belief that rests on specific facts. Beliefs live in the Wisdom layer and persist indefinitely.

## When to use

- You've synthesized multiple facts into a conclusion
- You're ready to take a position based on evidence
- "Based on [facts], I believe [conclusion]"

**The belief test:** Can you fill in "Based on [these facts], I believe [this]"? If not, it's a hunch—use `remember` instead.

## Tool call

```
believe(
  belief: "{your conclusion}",
  about: ["{node_ids of facts this rests on}"],  # REQUIRED
  confidence: 0.8,
  reasoning: "{why these facts lead to this belief}"
)
```

## Believe vs Hypothesize vs Commit

| Action | Confidence | Persistence |
|--------|------------|-------------|
| `hypothesize` | Low/medium | Session only |
| `believe` | High | Permanent |
| `commit` | Promotes hypothesis | Makes it permanent |

Use `hypothesize` when exploring. Use `believe` when you're confident from the start.

## No ceremony

Only believe what you've actually reasoned to. Don't manufacture beliefs for completeness.

---
name: engrammic:onboarding
description: Session start ritual. Load EAG guidance and check existing context.
---

# Onboarding

How to start a session with Engrammic memory.

## At session start

1. **Load your ICP guidance:**
   ```
   patterns(action: "get", name: "onboarding")
   ```
   This gives you ICP-tuned heuristics (coding, b2b-ops, etc.)

2. **Check existing context:**
   ```
   recall(query: "{what you're about to work on}")
   ```
   Ground yourself in what's already known.

3. **Proceed with the task.**

## The mental model

You have epistemically-grounded memory:

| Layer | What goes there | Evidence needed? |
|-------|-----------------|------------------|
| Memory | Observations, transient context | No |
| Knowledge | Verifiable facts | Yes |
| Wisdom | Synthesized beliefs | Cites facts |
| Intelligence | Reasoning chains | Session-only |
| Meta | Self-corrections | Links to nodes |

For full guidance, invoke `eag-guide`.

## No ceremony

This is a starting point, not a gate. If you already have context, skip to the work.

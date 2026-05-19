# Engrammic Skills

Open-source skills for AI agents using [Engrammic](https://engrammic.ai) epistemically-grounded memory.

## Installation

Copy skills to your agent's skills directory:

```bash
# Claude Code
cp -r engrammic:* ~/.claude/skills/

# Generic (works with Claude Code, Codex, Cursor, Windsurf, Gemini CLI)
cp -r engrammic:* ~/.agents/skills/
```

## Skills

### Cognitive Guide

| Skill | Trigger | Purpose |
|-------|---------|---------|
| `eag-guide` | "how should I use memory" | Mental model for EAG layers |

### Workflows

| Skill | Trigger | Purpose |
|-------|---------|---------|
| `debug` | debugging a bug | Track hypotheses, learn from resolution |
| `review` | reviewing code | Recall patterns, learn conventions |
| `investigate` | researching something | Gather evidence, reason to conclusion |
| `decide` | making a decision | Record options, commit with rationale |
| `checkpoint` | saving context | Summarize for later recall or handoff |
| `wander` | exploring a codebase | Curiosity-driven exploration |
| `explore-codebase` | systematic exploration | Parallel targeted + wanderer agents |

### Core Operations

| Skill | Layer | Purpose |
|-------|-------|---------|
| `observe` | memory | Store observation, no evidence needed |
| `learn` | knowledge | Store fact with evidence |
| `reason` | intelligence | Record reasoning steps |
| `reflect` | meta | Note when understanding changes |
| `connect` | link | Create typed relationship |
| `recall` | read | Search and retrieve |
| `trace` | read | Check provenance |

### Belief Operations

| Skill | Purpose |
|-------|---------|
| `belief-state` | Query current hypotheses |
| `update-belief` | Revise a hypothesis |
| `crystallize` | Promote hypothesis to commitment |
| `accept` | Accept a proposed belief |
| `reject` | Reject a proposed belief |

## Philosophy

These skills frontload guidance, then get out of your way. Use memory when it serves you, skip it when it doesn't. No ceremony required.

## License

MIT

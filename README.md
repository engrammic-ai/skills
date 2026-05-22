# Engrammic Skills

Workflow guidance for AI agents using Engrammic memory.

Skills teach your agent when and how to use memory. They frontload guidance, then get out of the way. Use memory when it serves you, skip it when it doesn't.

## Installation

```bash
# Claude Code
cp -r engrammic-* ~/.claude/skills/

# Cross-platform (Claude Code, Codex, Cursor, Windsurf, Gemini CLI)
cp -r engrammic-* ~/.agents/skills/
```

## Skills

### Session Start

| Skill | Trigger | Purpose |
|-------|---------|---------|
| `onboarding` | session start | Load guidance, check existing context |
| `patterns` | "how do I..." | Discover workflow templates |
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
| `remember` | memory | Store observation, no evidence needed |
| `learn` | knowledge | Store fact with evidence |
| `reason` | intelligence | Record reasoning steps |
| `reflect` | meta | Note when understanding changes |
| `connect` | link | Create typed relationship |
| `recall` | read | Search and retrieve |
| `trace` | read | Check provenance |

### Belief Operations

| Skill | Purpose |
|-------|---------|
| `hypothesize` | Form tentative belief |
| `believe` | Declare belief grounded in facts |
| `update-belief` | Revise a hypothesis |
| `crystallize` | Promote hypothesis to commitment |

## Learn More

- [Engrammic MCP](https://github.com/engrammic-ai/mcp) - hosted service
- [Engrammic Engine](https://github.com/engrammic-ai/engine) - local/offline
- [EAG Paradigm](https://github.com/engrammic-ai/primitives/blob/main/docs/README.md) - the cognitive architecture

## License

MIT

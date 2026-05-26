# Getting Started with Skills

## First Session

```
/engrammic-onboarding
```

Or using the patterns tool:
```
patterns(action: 'get', name: 'onboarding')
```

## How to Invoke

**Slash command** (if harness supports):
```
/engrammic-debug
/engrammic-checkpoint
```

**Patterns tool** (always works):
```
patterns(action: 'get', name: 'debug')
patterns(action: 'list')
patterns(action: 'search', query: 'belief')
```

## Verify Installation

```bash
ls ~/.claude/skills/engrammic-*
# or
patterns(action: 'list')
```

Should show 21+ skills.

## Recommended Order

1. **engrammic-onboarding** - session start, load context
2. **engrammic-eag-guide** - understand memory layers  
3. **engrammic-patterns** - discover workflow templates

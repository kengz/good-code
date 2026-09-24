# good-code

Agent instructions and coding standards built on [The 5 Principles](skills/good-code/PRINCIPLES.md): **Correct, Simple, General, Clear, Salient.**

> Framed for code — this repo is **good-code** — but medium-agnostic: the same five principles govern good writing, documentation, and design just as well.

## Install as Agent Skill

```bash
npx skills add kengz/good-code
```

This installs the `good-code` skill, which generates a project-specific `CLAUDE.md` (or `AGENTS.md`) tailored to your stack. Works with 37+ agents — Claude Code, Cursor, Codex, Copilot, and more.

## Use Directly

Copy [`skills/good-code/CLAUDE.md`](skills/good-code/CLAUDE.md) into your project root and adapt the comment blocks to your stack.

## What's Included

| File | Purpose |
|------|---------|
| [`PRINCIPLES.md`](skills/good-code/PRINCIPLES.md) | The 5 Principles — full explanations |
| [`CLAUDE.md`](skills/good-code/CLAUDE.md) | Agent instructions template |
| [`SKILL.md`](skills/good-code/SKILL.md) | Skill definition — auto-detects your stack and generates a tailored instructions file |

## The 5 Principles

1. **Correct** — Right in every state it can reach, failure included — constructed from known truths, not debugged into shape.
2. **Simple** — The fewest parts that lose nothing essential — complexity is not sophistication.
3. **General** — One principle that unifies many cases, in place of many ad hoc rules.
4. **Clear** — Says what it does — intent is obvious from naming and structure alone.
5. **Salient** — Reproducible, essential and lasting — independent attempts converge on it.

Read the full writeup in [`PRINCIPLES.md`](skills/good-code/PRINCIPLES.md).

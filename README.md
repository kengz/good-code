# good-code

Principles of good code design, and an agent skill that applies them. Built on [The 5 Principles](skills/good-code/PRINCIPLES.md): **Consistent, Simple, General, Clear, Salient.**

> Framed for code, but medium-agnostic: the same five principles govern good writing, documentation, and design just as well.

## Install as Agent Skill

```bash
npx skills add kengz/good-code
```

This installs the `good-code` skill. It detects your stack and generates a project-specific `AGENTS.md`, with `CLAUDE.md` as exactly `@AGENTS.md`. It works with many agents, including Claude Code, Cursor, Codex, and Copilot.

## Use Directly

Copy [`skills/good-code/CLAUDE.md`](skills/good-code/CLAUDE.md) into your project as `AGENTS.md`, adapt it to your stack, and make your `CLAUDE.md` the single line `@AGENTS.md`.

## What's Included

| File | Purpose |
|------|---------|
| [`PRINCIPLES.md`](skills/good-code/PRINCIPLES.md) | The principles, the premises, and the laws that follow from them |
| [`CLAUDE.md`](skills/good-code/CLAUDE.md) | Template for a project's `AGENTS.md` |
| [`SKILL.md`](skills/good-code/SKILL.md) | Skill definition: detects your stack and generates the instructions |

## The 5 Principles

1. **Consistent**: Agree with reality and with itself. Build from established facts, handle the conditions the work will actually meet, failure included, and let evidence decide what stands. No part contradicts another.
2. **Simple**: Use the fewest parts that preserve what matters; complexity is a cost, not evidence of sophistication.
3. **General**: Prefer one principle that covers related cases over a growing set of special rules.
4. **Clear**: Say what it does, so its purpose is obvious from its form alone.
5. **Salient**: Keep what is essential, reproducible, and likely to endure.

The Method (the Algorithm, Iteration, Identity, Refinement, Communication) is in [`PRINCIPLES.md`](skills/good-code/PRINCIPLES.md).

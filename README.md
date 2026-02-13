# good-code

Agent instructions and coding standards built on the [6 Principles of Good Code Design](skills/code-design/PRINCIPLES.md): **Consistent, Correct, Clear, Concise, Simple, Salient.**

## Install as Agent Skill

```bash
npx skills add kengz/good-code
```

This installs the `code-design` skill, which generates a project-specific `CLAUDE.md` (or `AGENTS.md`) tailored to your stack. Works with 37+ agents — Claude Code, Cursor, Codex, Copilot, and more.

## Use Directly

Copy [`skills/code-design/CLAUDE.md`](skills/code-design/CLAUDE.md) into your project root and adapt the comment blocks to your stack.

## What's Included

| File | Purpose |
|------|---------|
| [`PRINCIPLES.md`](skills/code-design/PRINCIPLES.md) | The 6 Principles — full explanations |
| [`CLAUDE.md`](skills/code-design/CLAUDE.md) | Agent instructions template |
| [`SKILL.md`](skills/code-design/SKILL.md) | Skill definition — auto-detects your stack and generates a tailored instructions file |

## The 6 Principles

1. **Consistent** — Design from first principles — unified naming, patterns, and conventions throughout.
2. **Correct** — Constructed from known truths, not debugged into shape.
3. **Clear** — Code does what it says — intent is obvious from naming and logic alone.
4. **Concise** — Simplified to the essence — nothing left to remove.
5. **Simple** — Few moving parts, easy to explain, cheap to maintain — complexity is not sophistication.
6. **Salient** — Essential enough to be used widely, fundamental enough to last.

Read the full writeup in [`PRINCIPLES.md`](skills/code-design/PRINCIPLES.md).

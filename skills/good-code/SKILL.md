---
name: good-code
description: >
  Generate a project-specific AGENTS.md (with CLAUDE.md as exactly `@AGENTS.md`) with coding standards, style guides, and
  best practices. Triggers on any request to set up a project, initialize coding standards,
  create or update CLAUDE.md or AGENTS.md, configure agent instructions, add code quality rules,
  or start a new codebase. Use this skill at the start of every new project.
---

# The 5 Principles: Agent Skill

You are setting up agent instructions for this project based on **The 5 Principles**: Consistent, Simple, General, Clear, Salient. Their laws (the Algorithm, Iteration, Self-improvement, Communication) are in `PRINCIPLES.md`.

## Step 1: Check for Existing Files

Before writing anything, check if any of these files already exist in the project root:
1. `CLAUDE.md`
2. `AGENTS.md`
3. `.cursorrules`
4. `.github/copilot-instructions.md`

If files exist, preserve project-specific rules and user work. Follow the authorized merge or replacement scope; ask only when that scope is unclear. Do not duplicate the shared rules or silently remove project requirements.

## Step 2: Detect Project Stack

Scan the project root for configuration files to determine the stack:

| File | Stack |
|------|-------|
| `package.json` | Node.js / TypeScript / JavaScript |
| `tsconfig.json` | TypeScript |
| `pyproject.toml` | Python (modern) |
| `setup.py` / `setup.cfg` | Python (legacy) |
| `Cargo.toml` | Rust |
| `go.mod` | Go |
| `Gemfile` | Ruby |
| `pom.xml` / `build.gradle` | Java / Kotlin |
| `mix.exs` | Elixir |
| `Package.swift` | Swift |

Also detect:
- **Package manager**: Look for `uv.lock`, `poetry.lock`, `pnpm-lock.yaml`, `yarn.lock`, `package-lock.json`, `Pipfile.lock`
- **Test framework**: Look for `pytest.ini`, `jest.config.*`, `vitest.config.*`, `.mocharc.*`, test directories
- **Linter/formatter**: Look for `.eslintrc.*`, `biome.json`, `ruff.toml`, `.prettierrc.*`, `rustfmt.toml`

## Step 3: Read the Template

Read the `CLAUDE.md` file located in this skill's directory (next to this SKILL.md file). This is the base template you will customize; its content becomes the project's `AGENTS.md`. Keep the principles' wording and the Algorithm's order (question, delete, simplify, accelerate, automate) as they are. For the full rationale behind each principle, see `PRINCIPLES.md` in the same directory.

## Step 4: Generate the Instructions File

Using the template from Step 3, create `AGENTS.md` in the project root, and make `CLAUDE.md` exactly the one line `@AGENTS.md` (Codification item 5 in `PRINCIPLES.md`). If the project already keeps its rules in `CLAUDE.md`, move them into `AGENTS.md`. Write the file in the Communication law's style: numbered lists, one idea per line, nested 4 spaces per level and at most three levels, plain words. The template includes Python and TypeScript as examples. Adapt the language-specific sections to match the detected stack:

1. **Style Guide**: Replace the Python/TypeScript subsections with idiomatic style entries for the detected language(s).
2. **Project Setup**: Replace with actual setup instructions: package manager commands, build/test/lint scripts found in the project's config files (`package.json` scripts, `Makefile`, `pyproject.toml`, etc.). The Python section in the template shows the level of detail expected.

## Step 5: Confirm

After writing the file, tell the user:
1. Which files were created and where
2. What stack was detected
3. What sections were customized
4. A suggestion they review and adjust the Project Setup section for any project-specific tooling

# The 5 Principles

> Framed for code, but medium-agnostic: the same five principles govern good writing, documentation, and design just as well.

Every rule in a codebase should derive from these axioms, except what the Premises admit directly. A rule that derives from neither does not belong. Each principle catches a failure the other four miss.

# Principles

## 1. Consistent

**Agree with reality and with itself.**

Build from established facts, handle the conditions the work will actually meet, failure included, and let evidence decide what stands. No part contradicts another.

1. **In code:** build upward from checked foundations; think through what can go wrong first; catch a failure early so it does the least harm.
2. **Catches:** code that holds in the expected case and fails, unnoticed, in the others.
3. **Measurable through:** claims traced to their basis, conditions handled, defects found after delivery, parts that contradict each other.

## 2. Simple

**Use the fewest parts that preserve what matters; complexity is a cost, not evidence of sophistication.**

Concision belongs here: remove duplication, dead work, and needless layers so the result can be explained and maintained.

1. **In code:** fewer parts leave fewer places for an error to hide; fewer dependencies mean lower upkeep.
2. **Catches:** code that is right but too large to hold in one mind, explain, or fix.
3. **Measurable through:** number of parts, dependencies, duplication, dead code, time to explain it.

## 3. General

**Prefer one principle that covers related cases over a growing set of special rules.**

When exceptions accumulate, find the rule beneath them. A supposed abstraction that adds unused machinery fails Simple.

1. **In code:** when special cases pile up, stop adding branches and look for the rule they are all instances of; the right one is shorter than what it replaces.
2. **Catches:** a growing set of special cases that no one rule yet explains.
3. **Measurable through:** special cases per rule, new rules per new requirement, abstractions with a single user.

## 4. Clear

**Say what it does, so its purpose is obvious from its form alone.**

Settle the terms and patterns first and use them everywhere: the same thing keeps the same name and shape, so a reader learns each pattern once.

1. **In code:** names and structure reveal intent; if code needs a separate explanation of what it is, it is not clear enough.
2. **Catches:** code that is right and small, and still hard to follow.
3. **Measurable through:** time for a newcomer to follow it, questions it raises, names used for one idea.

## 5. Salient

**Keep what is essential, reproducible, and likely to endure.**

A second independent attempt should reach the same result; if it cannot, the work may be polished but remains arbitrary or unverified.

1. **In code:** builds and tests give the same result from the repository alone, on any machine; nothing essential is missing and nothing inessential remains.
2. **Catches:** code that is neat and readable, and arbitrary, unrepeatable, or unverified.
3. **Measurable through:** agreement between independent attempts, the same result on a rebuild, churn, parts nobody uses.

# Premises

**Given, not derived: the boundary conditions every derivation starts from.**

1. **The owner decides** the purpose, the budget, the external commitments and which questions are worth asking, and ratifies changes to these rules.
2. **Authority boundaries and the owner's preferences enter as rules directly,** among them the Algorithm's order. Evidence still tests whether they hold.

# Method

**The laws, named so each can be cited; each derives from the principles.**

## 1. The Algorithm: how anything changes

In order:

1. **Question** every requirement; each names its owner and its reason.
2. **Delete** until something has to come back. Checks and authority boundaries are never deleted for speed.
3. **Simplify** what survives.
4. **Accelerate** it.
5. **Automate** last of all.

## 2. Iteration: how work moves

Plan a small step, build it, check it, land it, learn, repeat: progress is iterations times the gain of each. Measure it from the repository, on a clock, and compare its cost with the least the work needs.

## 3. Identity: how work stays traceable

1. Everything has one identity and one current owner, kept in the records and, once settled, in history. Act by that identity, never by a pattern, and hand over explicitly.
2. Resolve a reference against current truth when you use it.
3. An approval binds to the exact revision it approved.

## 4. Refinement: how knowledge improves

Any body of knowledge, these instructions included, iterates too: one body, tested by evidence.

1. **Notice** an anomaly (an error caught by review, a missed prediction, a needed exception, a repeat) and name it in the fixing commit.
2. **Classify** it: a misapplied rule gets a check, a wrong or missing rule is refined, and a misfit principle or premise goes to the owner.
3. **Absorb** a rule only if it fits the body: it covers its kind, contradicts nothing, and merges text.
4. **Unify** rules that share a cause into one law, on a regular clock.
5. **Verify**: keep a change only if its anomalies stop.

## 5. Communication: how anything is written

Every text: a reply, a code comment, a commit message, a document.

1. **Structure, never a wall.** One idea per line, in a numbered list so each item can be cited, with detail nested under its parent. Never pack a list into a paragraph, inline it as `(1)… (2)…`, or join it with `·` or `—`.
2. **Nest by 4 spaces per level, at most three levels;** a fourth level means the parent should be a heading.
3. **Plain words.** Explain it so a newcomer could follow. Write the finding, not a label for it; no acronyms, coined terms or stock phrases.

# Codification

**How the body is written down.**

1. **`AGENTS.md`:** the rules, identical across agents and providers.
2. **Skills:** the procedures. A file comes before a skill, and a script only for what is mechanical.
3. **History:** git history and commit trailers (`Key: value` lines). The instructions state the current rule; the incident behind it lives in history.
4. **Portable:** the same for every provider and every machine, resumable from the repository alone.
5. **Projects:** a project's `AGENTS.md` holds its rules and a short project section, and its `CLAUDE.md` is exactly `@AGENTS.md`.

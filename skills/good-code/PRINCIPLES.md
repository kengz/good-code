# The 5 Principles

> Framed for code — this repo is **good-code** — but medium-agnostic: the same five principles govern good writing, documentation, and design just as well.

Each principle catches a failure the other four miss. Reliable, Concise, Consistent and Reproducible are not separate principles; each lives inside the one it serves.

## 1. Correct

**Right in every state it can reach, failure included — constructed from known truths, not debugged into shape.**

Work should be constructed with the same rigor as a logical proof — built upward from solid foundations, where each layer is verified before the next is added. Defects are not inevitable; they are the consequence of loose construction. When every step is justified and every path is constrained, correctness is something you build from the start, not something you test into existence.

Correct includes **reliable**: correctness that holds under real conditions over time. A dropped connection, a crash, a restart — every failure state is designed for, not discovered later. When something fails, it fails safe and it fails visibly.

**Catches:** work that runs on the happy path and leaves a wrong state after a fault.

**Measurable through:** test coverage, defect density, failure-mode coverage, static analysis violations, type safety.

## 2. Simple

**The fewest parts that lose nothing essential — complexity is not sophistication.**

Complexity is not sophistication — it is bloat. A design with dozens of components and tangled dependencies is not a sign of intelligence; it is a sign of poor design that is expensive to maintain and impossible to explain. Nothing can hide in a simple thing, which is why it is more likely to be correct. It takes mastery to arrive at true simplicity. Fewer dependencies, lower maintenance, and lower cost follow as natural consequences.

Simple includes **concise**: every part justifies its existence. Eliminate duplication, remove what is dead, strip unnecessary abstraction. Brevity is about fewer *concepts* to hold in your head, not fewer characters — the goal is distillation, not minification.

**Catches:** work that is right but too large to hold in one mind, explain, or fix.

**Measurable through:** component count, dependency complexity, duplication, dead weight, ability to explain the system simply.

## 3. General

**One rule for the whole class of cases, not one rule per case.**

Build for the class, not the instance. A rule that covers many cases replaces many rules that each cover one, and a design of general parts stays small as the problem grows. When a new case arrives, the first question is whether an existing rule already covers it. Special cases accumulate quietly; each looks reasonable alone, and together they make the work incoherent.

Generality is bounded by simplicity: stop where going further would add parts nobody needs.

**Catches:** a pile of special cases, each tidy on its own.

**Measurable through:** special cases per rule, new rules per new requirement, parameters versus copies.

## 4. Clear

**Says what it does — intent is obvious from naming and structure alone.**

A lot of the work *is* naming. Names and structure should reveal intent immediately, with logic that follows naturally without mental gymnastics. If you need a comment to explain *what* something does, it is not clear enough. Clarity is not a courtesy — it is a responsibility to every future reader, and it has to be asked for, because it does not happen by default.

Clear includes **consistent**: establish naming conventions and structural patterns first, and apply them everywhere. When the same concept uses the same name everywhere, the work becomes searchable, replaceable, and predictable, and teaches its own rules the moment you touch it.

**Catches:** work that is correct and simple, and still unreadable.

**Measurable through:** cognitive complexity, nesting depth, unit length, naming convention adherence, pattern consistency across modules.

## 5. Salient

**Reproducible, essential and lasting — independent attempts converge on it.**

Salient includes **reproducible**, in two senses. Run it again and you get the same result. Derive it again, independently, and you arrive at the same thing. What is correct is rediscovered; what is arbitrary melts away. This is why mathematics and physics prize it, and it is the test to apply: would a second attempt, made alone, converge here?

Salient work is irreducible — nothing essential is missing, nothing inessential remains. It endures not because no one dares touch it, but because there is nothing left to improve.

**Catches:** work that is neat, broad and readable — and simply wrong, or impossible to repeat.

**Measurable through:** agreement between independent attempts, run-to-run determinism, churn, unused features.

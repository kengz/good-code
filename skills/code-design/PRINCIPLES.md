# Principles of Good Code Design

## 1. Consistent

**Design from first principles — unified naming, patterns, and conventions throughout.**

Consistency comes first. Before writing a single line, establish first principles: naming conventions, structural patterns, and standards that apply globally. When the same concept uses the same name everywhere, the codebase becomes searchable, replaceable, and predictable. Consistency creates a shared language across the entire system — developers navigate unfamiliar code with confidence because the system teaches you its own rules the moment you touch it.

**Measurable through:** naming convention adherence, code style consistency, pattern consistency across modules.

## 2. Correct

**Constructed from known truths, not debugged into shape.**

Code should be constructed with the same rigor as a logical proof — built upward from solid foundations, where each layer is verified before the next is added. Edge cases and error states are handled completely, not discovered later through debugging. Bugs are not inevitable; they are the consequence of loose construction. When every step is justified and every path is constrained, correctness is something you build from the start, not something you test into existence.

**Measurable through:** test coverage, bug density, static analysis violations, type safety.

## 3. Clear

**Code does what it says — intent is obvious from naming and logic alone.**

A lot of coding *is* naming. Function names, variable names, and structure should reveal intent immediately, with logic that follows naturally without mental gymnastics. If you need a comment to explain *what* code does, the code is not clear enough. Clarity is not a courtesy — it is a responsibility to every future reader.

**Measurable through:** cognitive complexity, cyclomatic complexity, nesting depth, method/function length, readability scores.

## 4. Concise

**Simplified to the essence — nothing left to remove.**

Every line of code must justify its existence. Conciseness is the discipline of relentless refactoring — eliminating duplication, removing dead code, and stripping unnecessary abstraction until only what matters remains. Brevity is about fewer *concepts* to hold in your head, not fewer characters. The goal is not minification; it is distillation. When code is concise, the cognitive load drops and the system becomes something a single mind can hold.

**Measurable through:** code duplication, lines of code, dead code, unused variables/imports.

## 5. Simple

**Few moving parts, easy to explain, cheap to maintain — complexity is not sophistication.**

Complexity is not sophistication — it is bloat. A complex architecture diagram with dozens of components and tangled dependencies is not a sign of intelligence; it is a sign of poor design that is expensive to maintain and impossible to explain. Good design is simple enough that anyone can understand it and reduced to the fewest moving parts while losing nothing essential. It takes mastery to arrive at true simplicity. Fewer dependencies, lower maintenance, and lower cost all follow as natural consequences.

**Measurable through:** component count, dependency complexity, ability to explain the system simply.

## 6. Salient

**Essential enough to be used widely, fundamental enough to last.**

The ultimate measure of good code is that it endures. Salient code addresses real needs, gets adopted widely, and stands unchanged over time — not because no one dares touch it, but because there is nothing left to improve. Code that follows the preceding principles — consistent, correct, clear, concise, and simple — naturally arrives here: used broadly, needed deeply, and lasting because it was built right.

**Measurable through:** code churn, unused features, technical debt ratio.

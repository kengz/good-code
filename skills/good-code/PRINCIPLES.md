# The 5 Principles

> Framed for code — this repo is **good-code** — but medium-agnostic: the same five principles govern good writing, documentation, and design just as well.

Each principle catches a failure the other four miss. Reliable, Concise, Consistent and Reproducible are not separate principles; each lives inside the one it serves.

## 1. Correct

**Right in every condition it will meet, failure included — constructed from known truths, not debugged into shape.**

Work should be constructed with the same rigor as a proof — built upward from solid foundations, where each step is checked before the next rests on it. Errors are not inevitable; they are the consequence of loose construction.

Correct includes **reliable**: correctness that holds in real conditions and over time, not only in the expected case. What can go wrong is thought through before it does. When something does fail, the failure is caught early and does the least harm.

**Catches:** work that holds in the expected case and fails, unnoticed, in the others.

**Measurable through:** claims traced to their basis, situations addressed, errors found after delivery, failures that were foreseen.

## 2. Simple

**The fewest parts that lose nothing essential — complexity is not sophistication.**

It is bloat. Work with many parts and tangled dependencies is not a sign of intelligence; it is a sign of poor design, expensive to maintain and impossible to explain. Fewer parts leave fewer places for an error to hide. It takes mastery to arrive at true simplicity. Fewer dependencies, lower upkeep and lower cost follow as natural consequences.

Simple includes **concise**: every part justifies its existence. Remove repetition, cut what no longer serves, drop layers that add nothing. Brevity is about fewer *ideas* to hold in your head, not fewer words — the goal is distillation, not compression.

**Catches:** work that is right but too large to hold in one mind, explain, or fix.

**Measurable through:** number of parts, dependencies, repetition, dead weight, time to explain it.

## 3. General

**One principle that unifies many cases, in place of many ad hoc rules.**

Ad hoc rules accumulate. Each fits its own case and looks reasonable alone; together they grow with the problem, overlap, and drift into contradiction. The better answer is almost always a more general principle — one that the ad hoc rules turn out to be special cases of, and that covers them all at once. Progress is the move from many rules to fewer, more general ones.

When rules start to pile up, stop adding and look for the principle underneath. A general principle does not grow as new cases arrive; the new case is already covered. The right one is also shorter than the rules it replaces, so generality and simplicity point the same way. Generalising that adds parts nobody needs is not generality — it fails Simple.

**Catches:** a growing set of ad hoc rules, each fitting its own case, that no one principle yet explains.

**Measurable through:** rules replaced per principle, special cases per rule, new rules per new requirement.

## 4. Clear

**Says what it does — its purpose is obvious from its form alone.**

Much of the work is choosing the right words and the right shape. Words and structure should reveal intent at once, and the reasoning should follow without effort. If it needs a separate explanation of *what* it is, it is not clear enough. Clarity is not a courtesy — it is a responsibility to everyone who reads, uses or maintains the work after you, and it has to be asked for, because it does not happen by default.

Clear includes **consistent**: settle the terms and patterns first, and apply them everywhere. When the same thing has the same name and the same shape wherever it appears, the work becomes predictable and easy to find your way in, and it teaches its own rules the moment you meet it.

**Catches:** work that is correct and simple, and still hard to follow.

**Measurable through:** time for a newcomer to follow it, questions it raises, names used for one idea, how many layers deep an idea sits.

## 5. Salient

**Reproducible, essential and lasting — independent attempts converge on it.**

Salient includes **reproducible**, twice over: repeatable and independently derivable. Do it again and you get the same result; derive it again, alone, and you arrive at the same thing. What is correct is rediscovered; what is arbitrary melts away. That is the test to apply: would a second attempt, made alone, converge here?

Salient work is irreducible — nothing essential is missing, nothing inessential remains. It endures not because no one dares touch it, but because there is nothing left to improve.

**Catches:** work that is neat, broad and readable — and simply wrong, or impossible to repeat.

**Measurable through:** agreement between independent attempts, the same result on repetition, churn, parts nobody uses.

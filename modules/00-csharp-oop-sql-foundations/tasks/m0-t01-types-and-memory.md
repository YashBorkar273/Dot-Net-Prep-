# M0-T01: Types and memory

| Status | Started | Completed | Best score |
|---|---|---|---|
| 🟨 In progress | 2026-11-25 | — | 9/10 |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Value vs reference type questions are the most common C# screening question at the junior level.

## Topics to cover
- [x] Value types vs reference types, stack vs heap (and why 'value types live on the stack' is only partly true)
- [x] Boxing and unboxing, and its cost
- [x] struct vs class vs record
- [x] String immutability, StringBuilder
- [x] Garbage collector: generations 0/1/2, LOH
- [x] IDisposable, using, finalizers, the dispose pattern

## Interview check: you must be able to answer
- What happens in memory when you assign one struct variable to another? A class variable?
- Why can boxing hurt performance in a loop?
- When does the GC run, and why do generations exist?
- Why do we need IDisposable if .NET has a garbage collector?

## Practice
Write a small console app that demonstrates copy semantics for a struct, a class and a record, and a class that implements IDisposable correctly. Add comments explaining each output line.

Put your code in `../solutions/m0-t01/` and your own notes in `../notes/m0-t01.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints (Q1, Q3, Q4 solid; Q2 pending re-check)
- [x] Practice reviewed by Claude: score **7/10 or higher** (9/10, 2026-11-25)
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|
| 2026-11-25 | Interview check | Q1 solid, Q2 not yet, Q3 solid, Q4 solid; Q2 re-ask assisted | Pending | Boxing: say "allocates + copies"; GC pressure means more frequent gen 0 collections, not a full heap |
| 2026-11-25 | Practice attempt 1 | 6.5/10 | Needs rework | Wrong ReferenceEquals prediction; no "why" comments; record demo showed `with`, not reference copy |
| 2026-11-25 | Practice attempt 2 | 9/10 | Ship it | All fixed; real verification of handle release; possible FileStream leak if the StreamWriter ctor throws |

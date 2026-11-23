# M0-T03: Generics, delegates, lambdas and events

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
LINQ, middleware and DI registration are all built on delegates and generics.

## Topics to cover
- [ ] Generic types and methods, constraints (where T : ...)
- [ ] Delegates, Func, Action, Predicate
- [ ] Lambdas and closures (including the captured-variable trap)
- [ ] Events and the observer pattern
- [ ] Extension methods

## Interview check: you must be able to answer
- What problem do generic constraints solve?
- What does a closure capture: the value or the variable?
- How is an event different from a public delegate field?
- How do extension methods make LINQ possible?

## Practice
Build a generic `Result<T>` type and an in-memory `Repository<T>` with a constraint, plus an extension method used on it.

Put your code in `../solutions/m0-t03/` and your own notes in `../notes/m0-t03.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

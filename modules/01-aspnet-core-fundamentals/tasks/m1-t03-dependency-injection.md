# M1-T03: Dependency injection

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
DI lifetimes are asked in nearly every .NET interview.

## Topics to cover
- [ ] Singleton, Scoped, Transient
- [ ] Captive dependency problem
- [ ] Resolving scoped services from singletons (IServiceScopeFactory)
- [ ] Registering interfaces, multiple implementations, keyed services
- [ ] Constructor injection vs service locator anti-pattern

## Interview check: you must be able to answer
- What goes wrong if a singleton depends on a scoped service?
- What lifetime should DbContext have, and why?
- Why is the service locator pattern considered an anti-pattern?

## Practice
Build a demo that prints instance IDs per lifetime across two requests, then reproduce and fix a captive dependency.

Put your code in `../solutions/m1-t03/` and your own notes in `../notes/m1-t03.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

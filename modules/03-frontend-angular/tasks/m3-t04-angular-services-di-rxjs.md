# M3-T04: Services, DI and RxJS

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
RxJS and subscription leaks are where Angular interviews separate juniors from mid-levels.

## Topics to cover
- [ ] Services, providedIn: 'root', inject()
- [ ] Angular DI vs ASP.NET Core DI
- [ ] Observables vs Promises
- [ ] Operators: map, filter, switchMap, mergeMap, catchError, debounceTime
- [ ] Unsubscribing, the async pipe, takeUntilDestroyed
- [ ] Signals vs RxJS: when to use which

## Interview check: you must be able to answer
- Observable vs Promise: give two real differences.
- switchMap vs mergeMap: which do you use for a search box, and why?
- How do memory leaks happen with subscriptions, and how do you prevent them?

## Practice
Build a search-as-you-type book search using a service, debounceTime and switchMap, with no leaked subscriptions.

Put your code in `../solutions/m3-t04/` and your own notes in `../notes/m3-t04.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

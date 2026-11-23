# M5-T01: Loading strategies and N+1

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
N+1 is the single most-asked EF Core performance question.

## Topics to cover
- [ ] Eager loading (Include/ThenInclude)
- [ ] Lazy loading and its risks
- [ ] Explicit loading
- [ ] N+1 detection and fixes
- [ ] Split queries vs cartesian explosion

## Interview check: you must be able to answer
- Explain N+1 and show two ways to fix it.
- When can Include make things worse?
- Why is lazy loading off by default in EF Core?

## Practice
Debugging drill: find and fix the N+1 and cartesian explosion in code Claude provides, showing SQL before and after.

Put your code in `../solutions/m5-t01/` and your own notes in `../notes/m5-t01.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

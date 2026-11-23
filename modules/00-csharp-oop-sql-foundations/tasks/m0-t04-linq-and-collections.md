# M0-T04: LINQ and collections

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Deferred execution misunderstandings cause real EF Core bugs later.

## Topics to cover
- [ ] Deferred vs immediate execution
- [ ] Common operators: Where, Select, SelectMany, GroupBy, Join, Any, First vs Single
- [ ] IEnumerable vs ICollection vs IList vs IQueryable (preview for EF)
- [ ] List, Dictionary, HashSet, Queue: Big-O of key operations
- [ ] yield return

## Interview check: you must be able to answer
- What happens if you enumerate a LINQ query twice?
- First vs FirstOrDefault vs Single: when does each throw?
- Why is Dictionary lookup O(1) on average, and what breaks that?
- What does `yield return` compile into?

## Practice
Solve 6 LINQ query exercises over an in-memory dataset Claude gives you, then explain where each query executes.

Put your code in `../solutions/m0-t04/` and your own notes in `../notes/m0-t04.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

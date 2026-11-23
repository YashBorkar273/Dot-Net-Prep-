# M5-T03: Bulk operations and raw SQL

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Updating 10,000 rows one by one is a classic performance blocker.

## Topics to cover
- [ ] ExecuteUpdate and ExecuteDelete
- [ ] FromSql / FromSqlInterpolated vs FromSqlRaw
- [ ] SQL injection risks
- [ ] SqlQuery for unmapped types

## Interview check: you must be able to answer
- Why is FromSqlRaw with string concatenation dangerous?
- What does ExecuteUpdate skip compared with SaveChanges?

## Practice
Implement a 'mark overdue loans' bulk operation two ways and compare.

Put your code in `../solutions/m5-t03/` and your own notes in `../notes/m5-t03.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

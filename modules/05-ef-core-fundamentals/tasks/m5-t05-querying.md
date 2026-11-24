# M5-T05: Querying with LINQ

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
IQueryable vs IEnumerable is a top-five EF interview question.

## Topics to cover
- [ ] How LINQ is translated to SQL
- [ ] IQueryable vs IEnumerable (where filtering happens)
- [ ] Client vs server evaluation
- [ ] Projections with Select
- [ ] Logging generated SQL

## Interview check: you must be able to answer
- What's the difference between calling .Where() before and after .ToList()?
- Why does projecting to a DTO often produce better SQL?
- How do you see the SQL EF Core generates?

## Practice
Write 6 queries Claude specifies and paste the generated SQL for each with comments.

Put your code in `../solutions/m5-t05/` and your own notes in `../notes/m5-t05.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

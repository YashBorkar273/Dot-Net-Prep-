# M0-T07: SQL essentials

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
You can't reason about EF Core performance without knowing what SQL it produces.

## Topics to cover
- [ ] SELECT, JOIN types (inner, left, cross), GROUP BY/HAVING
- [ ] Primary and foreign keys, normalisation (1NF to 3NF)
- [ ] Indexes: clustered vs non-clustered, when they help and hurt
- [ ] Transactions, ACID, isolation levels (awareness)
- [ ] Reading an execution plan (basics)

## Interview check: you must be able to answer
- Inner join vs left join: give a case where the choice changes the result.
- Why not index every column?
- What does a transaction guarantee?
- What is the N+1 query problem in plain SQL terms?

## Practice
Design a schema for a small library system and write 6 queries Claude specifies.

Put your code in `../solutions/m0-t07/` and your own notes in `../notes/m0-t07.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

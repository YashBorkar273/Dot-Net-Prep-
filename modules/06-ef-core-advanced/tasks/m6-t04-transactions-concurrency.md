# M6-T04: Transactions and concurrency

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Concurrency questions separate people who've thought about real users from those who haven't.

## Topics to cover
- [ ] SaveChanges is transactional by default
- [ ] Explicit transactions
- [ ] Optimistic concurrency with rowversion/concurrency tokens
- [ ] Handling DbUpdateConcurrencyException

## Interview check: you must be able to answer
- Two users edit the same book at the same time. What happens by default, and how do you fix it?
- When do you need an explicit transaction?

## Practice
Add optimistic concurrency to book updates and return 409 on conflicts.

Put your code in `../solutions/m6-t04/` and your own notes in `../notes/m6-t04.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

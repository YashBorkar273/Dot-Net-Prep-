# M5-T06: Change tracking and SaveChanges

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Explains 'why didn't my update save?' and 'why is this so slow?' bugs.

## Topics to cover
- [ ] Entity states: Added, Modified, Unchanged, Deleted, Detached
- [ ] How SaveChanges builds commands
- [ ] Tracking vs no-tracking queries
- [ ] Attach vs Update, disconnected entities

## Interview check: you must be able to answer
- What happens if you call Update() on an entity where only one field changed?
- When should a query be AsNoTracking?

## Practice
Debugging drill: Claude gives you 4 update scenarios that misbehave. Explain and fix each.

Put your code in `../solutions/m5-t06/` and your own notes in `../notes/m5-t06.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

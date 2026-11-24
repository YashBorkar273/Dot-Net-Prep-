# M5-T04: Migrations

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Migrations in production is a common 'how would you deploy this' question.

## Topics to cover
- [ ] Add, remove, update database
- [ ] What a migration file contains, the model snapshot
- [ ] Generating SQL scripts and idempotent scripts
- [ ] Applying migrations in production (and why not at app startup)
- [ ] Seeding data

## Interview check: you must be able to answer
- Why is calling Database.Migrate() at startup risky in production?
- Two developers add migrations on separate branches. What happens?

## Practice
Create the initial migration, generate an idempotent SQL script, and seed data.

Put your code in `../solutions/m5-t04/` and your own notes in `../notes/m5-t04.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

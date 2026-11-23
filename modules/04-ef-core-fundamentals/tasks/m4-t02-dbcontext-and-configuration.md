# M4-T02: DbContext and model configuration

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Configuration mistakes cause most first-time EF bugs.

## Topics to cover
- [ ] DbContext and DbSet
- [ ] Registering DbContext and its lifetime
- [ ] Conventions vs data annotations vs Fluent API
- [ ] IEntityTypeConfiguration<T>
- [ ] Keys, required, max length, indexes

## Interview check: you must be able to answer
- Why is DbContext not thread-safe, and what does that mean for DI lifetime?
- When must you use Fluent API instead of annotations?

## Practice
Create the Library DbContext with Fluent API configuration classes.

Put your code in `../solutions/m4-t02/` and your own notes in `../notes/m4-t02.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

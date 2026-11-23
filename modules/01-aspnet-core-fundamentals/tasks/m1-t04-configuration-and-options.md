# M1-T04: Configuration and the Options pattern

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Every real app needs config per environment, and secrets handling reveals your maturity.

## Topics to cover
- [ ] Configuration providers and their precedence
- [ ] appsettings.{Environment}.json
- [ ] User secrets and environment variables
- [ ] IOptions vs IOptionsSnapshot vs IOptionsMonitor
- [ ] Options validation (ValidateDataAnnotations, ValidateOnStart)

## Interview check: you must be able to answer
- If a key exists in appsettings.json and an environment variable, which wins?
- When do you need IOptionsMonitor over IOptions?
- Where should a database password live in development? In production?

## Practice
Bind a strongly-typed settings class with validation that fails fast on startup.

Put your code in `../solutions/m1-t04/` and your own notes in `../notes/m1-t04.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

# M1-T01: Hosting, Program.cs and the request lifecycle

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
You'll be asked to walk through what happens when a request hits your app.

## Topics to cover
- [ ] WebApplication builder, the generic host
- [ ] Kestrel and reverse proxies
- [ ] Program.cs structure: services vs pipeline
- [ ] Request lifecycle end to end

## Interview check: you must be able to answer
- Walk me through what happens from an HTTP request arriving to a response leaving.
- What is Kestrel and why put a reverse proxy in front of it?
- What is the difference between builder.Services and app.Use...?

## Practice
Create an empty ASP.NET Core app and annotate Program.cs explaining every line.

Put your code in `../solutions/m1-t01/` and your own notes in `../notes/m1-t01.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

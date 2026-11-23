# M1-T05: Logging and environments

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Structured logging separates juniors who debug with Console.WriteLine from those ready for production.

## Topics to cover
- [ ] ILogger<T>, log levels, filtering
- [ ] Structured logging and message templates
- [ ] Why not string interpolation in log calls
- [ ] Environments: Development/Staging/Production

## Interview check: you must be able to answer
- Why is `_logger.LogInformation($"User {id}")` worse than a message template?
- How do you change log levels without redeploying?

## Practice
Add structured logging to your middleware from task 02 with correct levels.

Put your code in `../solutions/m1-t05/` and your own notes in `../notes/m1-t05.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

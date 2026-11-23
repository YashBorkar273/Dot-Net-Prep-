# M2-T04: DTOs, mapping and error handling

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Returning EF entities directly from an API is a classic blocker in code reviews.

## Topics to cover
- [ ] Request/response DTOs vs entities
- [ ] Manual mapping vs mapping libraries (and the trade-offs)
- [ ] ProblemDetails (RFC 9457)
- [ ] Global exception handling with IExceptionHandler / UseExceptionHandler
- [ ] Not leaking stack traces

## Interview check: you must be able to answer
- Give three reasons not to return entities from an API.
- How do you return consistent errors from every endpoint?
- Where should a 'not found' decision be made: controller or service?

## Practice
Introduce DTOs and a global exception handler producing ProblemDetails.

Put your code in `../solutions/m2-t04/` and your own notes in `../notes/m2-t04.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

# M2-T01: REST and HTTP semantics

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Wrong status codes and verbs are the first thing a reviewer notices.

## Topics to cover
- [ ] Resources and URIs
- [ ] HTTP verbs, safety and idempotency
- [ ] Status codes: 200/201/204/400/401/403/404/409/422/500
- [ ] Headers: Location, ETag, Cache-Control

## Interview check: you must be able to answer
- Is PUT idempotent? POST? PATCH?
- 401 vs 403?
- What should a successful POST that creates a resource return?

## Practice
Design (on paper) the endpoints for a library API: routes, verbs, status codes and bodies.

Put your code in `../solutions/m2-t01/` and your own notes in `../notes/m2-t01.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

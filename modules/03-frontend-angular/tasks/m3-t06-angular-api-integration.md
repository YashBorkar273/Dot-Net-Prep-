# M3-T06: HTTP and API integration

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
This is the full-stack part: frontend and backend working together correctly.

## Topics to cover
- [ ] HttpClient and typed responses
- [ ] HTTP interceptors: attaching JWT, global error handling
- [ ] Environment configuration
- [ ] Loading, empty and error states
- [ ] Login flow end to end with ASP.NET Core JWT
- [ ] CORS configuration in ASP.NET Core

## Interview check: you must be able to answer
- Walk me through what happens from clicking Login to calling a protected endpoint.
- What should the UI do when the API returns 401? 403? 500?
- Why use an interceptor instead of adding headers in each service?

## Practice
Connect the Angular app to your Library API with login, an auth interceptor and proper error handling.

Put your code in `../solutions/m3-t06/` and your own notes in `../notes/m3-t06.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

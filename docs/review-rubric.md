# Code Review Rubric

Every coding submission is scored out of 10, like a pull request at a company with a real review culture. Feedback is blunt: the goal is to find what an interviewer or senior reviewer would find, before they do.

## Categories
| Category | Points | What gets checked |
|---|---|---|
| Correctness and edge cases | 2.0 | Meets requirements; nulls, empty inputs, not-found, duplicates, boundaries |
| Design and separation of concerns | 1.5 | Thin controllers, logic in services, no god classes, sensible abstractions, SOLID |
| Data access | 1.5 | No N+1, projections, AsNoTracking for reads, no loading whole tables, correct DbContext lifetime, transactions where needed |
| API contract and HTTP semantics | 1.0 | Correct verbs and status codes, DTOs (never entities), ProblemDetails, pagination on lists |
| Error handling and validation | 1.0 | Validation at the boundary, no swallowed exceptions, global handler, no leaked stack traces |
| Security | 1.0 | No SQL injection, no secrets in code, authZ on sensitive endpoints, no over-posting, input limits |
| Idiomatic C# / .NET | 1.0 | Async all the way with CancellationToken, DI over `new`, naming conventions, nullable annotations, modern C# |
| Testing | 1.0 | Tests exist, test behaviour not implementation, cover edge cases. For tasks before Module 6 without required tests, this point is awarded for testable design |

## Frontend (Angular/React) submissions
Same 10 points, with three categories reinterpreted:
- **Data access → State and data flow (1.5):** no leaked subscriptions (async pipe / takeUntilDestroyed), no duplicated state, sensible signals/RxJS use, OnPush where it fits.
- **API contract → API integration (1.0):** typed models, interceptors for auth and errors, loading/empty/error states handled.
- **Security (1.0):** no tokens in unsafe places without justification, no `innerHTML` with untrusted data, guards treated as UX only (the API still enforces authZ).

## Severity labels
- 🔴 **Blocker**: wrong, insecure, loses data, or fails a requirement. **Any blocker caps the score at 4/10.**
- 🟠 **Major**: works but would be rejected in review (N+1, entity returned from API, sync-over-async, missing validation).
- 🟡 **Minor**: naming, readability, small inefficiencies.
- ⚪ **Nit**: style preference, optional.
- 🟢 **Praise**: something done right, named specifically so you repeat it.

## Score to verdict
| Score | Verdict | Meaning |
|---|---|---|
| 9-10 | Ship it | Senior reviewer approves as-is |
| 7-8 | Minor changes | Solid mid-level work; approve after small fixes. **Minimum to complete a task.** |
| 5-6 | Needs rework | Core issues; fix and resubmit |
| 0-4 | Not yet | Approach or concept gap; revisit the concept before resubmitting |

## Concept answers
Interview-check and test answers are graded **strong** (correct, precise, explains why), **solid** (correct, minor gaps), **assisted** (needed a hint), or **not yet**. Only strong and solid count toward completion.

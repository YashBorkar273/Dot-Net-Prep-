# M2-T03: Model binding and validation

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Validation gaps are security and data-quality bugs.

## Topics to cover
- [ ] [FromBody], [FromRoute], [FromQuery], [FromHeader], [FromServices]
- [ ] Automatic 400 responses
- [ ] DataAnnotations vs FluentValidation
- [ ] Validating at the boundary

## Interview check: you must be able to answer
- Where does model binding look for a parameter by default?
- What happens to an invalid model under [ApiController]?
- Why not validate inside the entity only?

## Practice
Add validation to your create/update endpoints with meaningful error responses.

Put your code in `../solutions/m2-t03/` and your own notes in `../notes/m2-t03.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

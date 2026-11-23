# M0-T05: Async and await

| Status | Started | Completed | Best score |
|---|---|---|---|
| ⬜ Not started | — | — | — |

> Status legend: ⬜ Not started · 🟨 In progress · ✅ Completed · 🔁 Needs revision. Only Claude marks ✅, and only after the completion criteria below are met in a session.

## Why this matters
Every API action is async. Misusing async is the #1 red flag in .NET code reviews.

## Topics to cover
- [ ] Task vs Thread, I/O-bound vs CPU-bound
- [ ] What the compiler generates (state machine)
- [ ] async void and why to avoid it
- [ ] Deadlocks from .Result/.Wait()
- [ ] ConfigureAwait(false) and why ASP.NET Core differs
- [ ] CancellationToken
- [ ] Task.WhenAll vs sequential awaits
- [ ] ValueTask (awareness)

## Interview check: you must be able to answer
- Does `await` create a new thread?
- Why can `.Result` deadlock in some apps but usually not in ASP.NET Core?
- When would you use Task.WhenAll?
- How should a cancelled HTTP request stop a database query?

## Practice
Debugging drill: Claude gives you broken async code with 4 bugs. Find, fix and explain each.

Put your code in `../solutions/m0-t05/` and your own notes in `../notes/m0-t05.md`.

## Completion criteria
- [ ] Interview check answered in a session: every question **solid** or **strong**, without hints
- [ ] Practice reviewed by Claude: score **7/10 or higher**
- [ ] Notes written in your own words

## Review log
| Date | Activity | Score / Result | Verdict | Key feedback |
|---|---|---|---|---|

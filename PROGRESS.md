# Progress: .NET Interview Prep

<!-- Last saved: 2026-11-25 | Source of truth for this learning journey. Only Claude updates evidence, XP and statuses, and only for things that happened in a session. -->

## Dashboard
| Level | XP | Streak | Current module | Current task | Tasks completed | Due for revision |
|---|---|---|---|---|---|---|
| 1 Novice | 152 | 1 day | Module 0 | M0-T01 (boxing re-check + notes), then M0-T02 | 0 / 54 | 3 due 2026-11-26 |

## Roadmap status
| Module | Status | Tasks done | Module test |
|---|---|---|---|
| Module 0: C#, OOP and SQL Foundations | 🟨 In progress | 0/7 | not attempted |
| Module 1: ASP.NET Core Fundamentals | ⬜ Not started | 0/5 | not attempted |
| Module 2: Web API | ⬜ Not started | 0/7 | not attempted |
| Module 3: Frontend: TypeScript and Angular (React comparison) | ⬜ Not started | 0/8 | not attempted |
| Module 4: MVC | ⬜ Not started | 0/4 | not attempted |
| Module 5: ORM Concepts and EF Core Fundamentals | ⬜ Not started | 0/7 | not attempted |
| Module 6: EF Core Advanced and Performance | ⬜ Not started | 0/5 | not attempted |
| Module 7: Production Concerns | ⬜ Not started | 0/6 | not attempted |
| Capstone: Capstone and final mock interview | ⬜ Not started | 0/5 | not attempted |

## Mastery map
<!-- Levels: 0 Not started · 1 Introduced · 2 Understands · 3 Applies · 4 Proficient · 5 Mastered. Rows are added as concepts are taught. "(unverified)" = self-reported. -->
| Concept | Task | Level | Target | Last evidence | Next revision |
|---|---|---|---|---|---|
| Value vs reference type copy semantics | M0-T01 | 3 | 4 | 2026-11-25 interview check solid + practice 9/10 | 2026-11-26 |
| Where values live (inline in their container, not "structs on the stack") | M0-T01 | 2 | 4 | 2026-11-25 array-of-structs check (assisted) | — |
| Boxing/unboxing and GC pressure | M0-T01 | 2 | 4 | 2026-11-25 interview Q2 not yet, re-ask assisted; practice correct | — |
| class vs record vs struct equality | M0-T01 | 3 | 4 | 2026-11-25 check strong + practice 9/10 | 2026-11-26 |
| String immutability, StringBuilder | M0-T01 | 2 | 4 | 2026-11-25 check assisted | — |
| GC generations, LOH | M0-T01 | 2 | 4 | 2026-11-25 interview Q3 solid, LOH check solid | — |
| IDisposable, using, deterministic cleanup | M0-T01 | 3 | 4 | 2026-11-25 interview Q4 solid + practice 9/10 + defended Dispose ordering | 2026-11-26 |
| LINQ deferred execution | M0-T04 | 2 | 4 | 2026-11-25 diagnostic (solid) | — |
| Dependency Inversion / constructor injection | M0-T02 | 2 | 4 | 2026-11-25 diagnostic (solid) | — |
| Async/await in ASP.NET Core (sync-over-async) | M0-T05 | 0 | 4 | 2026-11-25 diagnostic (not yet) | — |
| IQueryable vs IEnumerable / where EF filtering runs | M0-T04, M5-T05 | 0 | 4 | 2026-11-25 diagnostic (not yet) | — |

## Evidence log
| Date | Task / concept | Evidence type | What the learner did | Result | Level / status change |
|---|---|---|---|---|---|
| 2026-11-25 | Value vs reference types | Diagnostic | Predicted `1 10` for struct vs class copy; reason given as value vs reference type, without explaining what gets copied | solid | 0 → 2 |
| 2026-11-25 | LINQ deferred execution | Diagnostic | Predicted 3 and named deferred execution | solid | 0 → 2 |
| 2026-11-25 | Async/await (sync-over-async) | Diagnostic | Saw that `.Result` blocks, but called it a "concurrency" issue; missed thread-pool starvation; rewrite didn't compile (`Aysnc`, return type not `Task<IActionResult>`) | not yet | stays 0 |
| 2026-11-25 | IQueryable vs IEnumerable | Diagnostic | Said version B returns IQueryable (it returns List); missed that version A loads the whole table and filters in memory | not yet | stays 0 |
| 2026-11-25 | DIP / constructor injection | Diagnostic | Named DIP and testability; correct refactor to interface + constructor injection; didn't mention DI registration or why testing gets easier | solid | 0 → 2 |
| 2026-11-25 | Where struct fields live | Diagnose probe | Said fields of a class object live on the stack | not yet (teaching probe) | — |
| 2026-11-25 | Arrays are reference types | Check | Predicted 5 and identified Point[] as a reference type | solid | — |
| 2026-11-25 | Array of structs location | Check | After step-down: one heap object with 3 inline values | assisted | 0 → 2 |
| 2026-11-25 | Boxing copy | Check | Predicted 42; explained the copy when asked for the why | solid | — |
| 2026-11-25 | class vs record equality | Check | false/true/false with correct reasons | strong | — |
| 2026-11-25 | String immutability | Check | Right output, wrong reason (said `b = a` creates a new string); fixed after a ReferenceEquals nudge | assisted | 0 → 2 |
| 2026-11-25 | LOH | Check | LOH, gen 2, fragmentation; missed gen 2 GC triggering, said objects "survive one collection" | solid | — |
| 2026-11-25 | IDisposable consequences | Check | Correct `using` fix; wrong consequence ("heap is full") | not yet (consequence) | — |
| 2026-11-25 | M0-T01 interview Q1 (copy semantics) | Interview check | Correct with examples; missed shallow copy; invalid initializer syntax | solid | → 3 with practice |
| 2026-11-25 | M0-T01 interview Q2 (boxing in a loop) | Interview check | Said boxing "fills the entire heap"; no fix given | not yet | — |
| 2026-11-25 | M0-T01 interview Q3 (GC) | Interview check | Triggers and generational reasoning correct; follow-up on promotion slightly fuzzy | solid | 0 → 2 |
| 2026-11-25 | M0-T01 interview Q4 (IDisposable) | Interview check | Correct core; missed determinism; called a connection string a resource | solid (low end) | — |
| 2026-11-25 | M0-T01 interview Q2 re-ask | Interview check | Correct mechanism, but mirrored the model answer just given; didn't name boxing | assisted | — |
| 2026-11-25 | M0-T01 practice attempt 1 | Code review (read, not run) | Console demo: wrong ReferenceEquals prediction, missing reasons, misleading record demo | 6.5/10 Needs rework | — |
| 2026-11-25 | M0-T01 practice attempt 2 | Code review (read, not run) | All findings fixed; real verification with FileShare.None + ReadAllText/Delete | 9/10 Ship it | → 3 |
| 2026-11-25 | Dispose ordering | Defend-your-code | Explained why `_disposed = true` goes before `_writer.Dispose()` | strong | — |

## Weak areas and misconceptions
| Since | Concept / misconception | Signals | Remediation plan | Status |
|---|---|---|---|---|
| 2026-11-25 | Blocking on async (`.Result`) understood as "concurrency" rather than thread blocking / thread-pool starvation; async method signatures | Diagnostic Q3 | Teach in M0-T05 (Task vs thread, what await does); debugging drill | open (diagnostic gap) |
| 2026-11-25 | Doesn't yet know where an EF query executes (database vs memory); unclear on IQueryable vs IEnumerable vs List | Diagnostic Q4 | Preview in M0-T04, full treatment in M5-T05 with generated SQL | open (diagnostic gap) |
| 2026-11-25 | "Structs live on the stack" | Diagnose probe, then array-of-structs check (same mistake twice) | Re-check in revision with a struct-inside-class and a captured-local example | improving |
| 2026-11-25 | Treats the heap as a bucket that "fills up"; mixes up memory with OS resources | StreamReader consequence, interview Q2 | Re-ask boxing (new wording) next session; explain GC pressure vs leaks | open |

## Revision queue
<!-- Intervals after a concept reaches level 3: +1, +3, +7, +14, +30 days. -->
| Concept | Interval step | Due | Last result |
|---|---|---|---|
| Value vs reference type copy semantics | +1 | 2026-11-26 | practice 9/10 |
| class vs record vs struct equality | +1 | 2026-11-26 | practice 9/10 |
| IDisposable, using, deterministic cleanup | +1 | 2026-11-26 | practice 9/10 |

## XP ledger
| Date | Activity | XP |
|---|---|---|
| 2026-11-25 | Diagnostic Q1 (solid) | 7 |
| 2026-11-25 | Diagnostic Q2 (solid) | 7 |
| 2026-11-25 | Diagnostic Q3 (not yet) | 0 |
| 2026-11-25 | Diagnostic Q4 (not yet) | 0 |
| 2026-11-25 | Diagnostic Q5 (solid) | 7 |
| 2026-11-25 | Check: arrays are reference types (solid) | 7 |
| 2026-11-25 | Check: array of structs (assisted) | 3 |
| 2026-11-25 | Check: boxing copy (solid) | 7 |
| 2026-11-25 | Check: record equality (strong) | 10 |
| 2026-11-25 | Check: string immutability (assisted) | 3 |
| 2026-11-25 | Check: LOH (solid) | 7 |
| 2026-11-25 | Check: IDisposable consequence (not yet) | 0 |
| 2026-11-25 | M0-T01 interview Q1 (solid) | 7 |
| 2026-11-25 | M0-T01 interview Q2 (not yet) | 0 |
| 2026-11-25 | M0-T01 interview Q3 (solid) | 7 |
| 2026-11-25 | M0-T01 interview Q4 (solid) | 7 |
| 2026-11-25 | M0-T01 interview Q2 re-ask (assisted) | 3 |
| 2026-11-25 | M0-T01 practice, final verdict Ship it (60 × 1.0) | 60 |
| 2026-11-25 | Defend-your-code: Dispose ordering (strong) | 10 |
| | **Total** | **152** |

## Achievements
| Date | Achievement | Earned by |
|---|---|---|
| 2026-11-25 | First Steps | Completed discovery and the 5-question diagnostic |
| 2026-11-25 | Comeback | M0-T01 practice: 6.5/10 Needs rework → 9/10 Ship it |

## Roadmap changes
| Date | Change | Reason |
|---|---|---|
| 2026-11-25 | Module 0 made mandatory; OOP/SOLID and SQL essentials added | Under 1 year of experience; junior interviews weigh C#/OOP fundamentals heavily, and EF Core needs SQL |
| 2026-11-25 | Modules 6-7 (EF advanced, production) targeted at "explain and spot the problem" depth; mock interviews after Modules 2, 6 and the capstone | Goal is interview prep at junior/mid level |
| 2026-11-25 | Added Module 3: Frontend (TypeScript + Angular, React comparison); MVC, EF Core and later modules renumbered 4-7; capstone becomes full-stack | Target role is full-stack Software Engineer; Angular chosen as primary |
| 2026-11-25 | Kept MVC and production modules at full depth; estimated length ~15 weeks | Deadline is tentative; learner prioritises learning depth over speed |

## Session log
| Date | Covered | Results | Next steps |
|---|---|---|---|
| 2026-11-25 | Agreed scope and roadmap; captured goal (interview prep), experience (<1 year), time (5-10 h/week); set up repo and CLAUDE.md; captured role (full-stack SE), tentative 3-month timeframe, Angular as primary frontend; added frontend module | No assessed work yet | — |
| 2026-11-25 | Captured IDE (Visual Studio) and database (SQL Server); ran 5-question diagnostic | 3 solid, 2 not yet; gaps in async and EF query execution; 21 XP | Start M0-T01 (fast pace on basics); give extra weight to M0-T04 and M0-T05 |
| 2026-11-25 | M0-T01 Types and memory: taught where values live, boxing, records, strings, GC, IDisposable; interview check; practice reviewed twice | Interview Q1/Q3/Q4 solid, Q2 not yet (assisted on re-ask); practice 6.5 → 9/10; +131 XP; 2 misconceptions logged | Re-check boxing/GC pressure (new wording) with no hints; confirm notes in notes/m0-t01.md; revise 3 items due 2026-11-26; then M0-T02 |

## Self-reported (unverified)
| Date | Claim | Status |
|---|---|---|
| 2026-11-25 | Under 1 year hands-on .NET experience | Context only, no credit |

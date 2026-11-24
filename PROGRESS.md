# Progress: .NET Interview Prep

<!-- Last saved: 2026-11-23 | Source of truth for this learning journey. Only Claude updates evidence, XP and statuses, and only for things that happened in a session. -->

## Dashboard
| Level | XP | Streak | Current module | Current task | Tasks completed | Due for revision |
|---|---|---|---|---|---|---|
| 1 Novice | 21 | 1 day | Module 0 | M0-T01 Types and memory | 0 / 54 | 0 |

## Roadmap status
| Module | Status | Tasks done | Module test |
|---|---|---|---|
| Module 0: C#, OOP and SQL Foundations | ⬜ Not started | 0/7 | not attempted |
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
| Value vs reference type copy semantics | M0-T01 | 2 | 4 | 2026-11-23 diagnostic (solid) | — |
| LINQ deferred execution | M0-T04 | 2 | 4 | 2026-11-23 diagnostic (solid) | — |
| Dependency Inversion / constructor injection | M0-T02 | 2 | 4 | 2026-11-23 diagnostic (solid) | — |
| Async/await in ASP.NET Core (sync-over-async) | M0-T05 | 0 | 4 | 2026-11-23 diagnostic (not yet) | — |
| IQueryable vs IEnumerable / where EF filtering runs | M0-T04, M5-T05 | 0 | 4 | 2026-11-23 diagnostic (not yet) | — |

## Evidence log
| Date | Task / concept | Evidence type | What the learner did | Result | Level / status change |
|---|---|---|---|---|---|
| 2026-11-23 | Value vs reference types | Diagnostic | Predicted `1 10` for struct vs class copy; reason given as value vs reference type, without explaining what gets copied | solid | 0 → 2 |
| 2026-11-23 | LINQ deferred execution | Diagnostic | Predicted 3 and named deferred execution | solid | 0 → 2 |
| 2026-11-23 | Async/await (sync-over-async) | Diagnostic | Saw that `.Result` blocks, but called it a "concurrency" issue; missed thread-pool starvation; rewrite didn't compile (`Aysnc`, return type not `Task<IActionResult>`) | not yet | stays 0 |
| 2026-11-23 | IQueryable vs IEnumerable | Diagnostic | Said version B returns IQueryable (it returns List); missed that version A loads the whole table and filters in memory | not yet | stays 0 |
| 2026-11-23 | DIP / constructor injection | Diagnostic | Named DIP and testability; correct refactor to interface + constructor injection; didn't mention DI registration or why testing gets easier | solid | 0 → 2 |

## Weak areas and misconceptions
| Since | Concept / misconception | Signals | Remediation plan | Status |
|---|---|---|---|---|
| 2026-11-23 | Blocking on async (`.Result`) understood as "concurrency" rather than thread blocking / thread-pool starvation; async method signatures | Diagnostic Q3 | Teach in M0-T05 (Task vs thread, what await does); debugging drill | open (diagnostic gap) |
| 2026-11-23 | Doesn't yet know where an EF query executes (database vs memory); unclear on IQueryable vs IEnumerable vs List | Diagnostic Q4 | Preview in M0-T04, full treatment in M5-T05 with generated SQL | open (diagnostic gap) |

## Revision queue
<!-- Intervals after a concept reaches level 3: +1, +3, +7, +14, +30 days. -->
| Concept | Interval step | Due | Last result |
|---|---|---|---|

## XP ledger
| Date | Activity | XP |
|---|---|---|
| 2026-11-23 | Diagnostic Q1 (solid) | 7 |
| 2026-11-23 | Diagnostic Q2 (solid) | 7 |
| 2026-11-23 | Diagnostic Q3 (not yet) | 0 |
| 2026-11-23 | Diagnostic Q4 (not yet) | 0 |
| 2026-11-23 | Diagnostic Q5 (solid) | 7 |
| | **Total** | **21** |

## Achievements
| Date | Achievement | Earned by |
|---|---|---|
| 2026-11-23 | First Steps | Completed discovery and the 5-question diagnostic |

## Roadmap changes
| Date | Change | Reason |
|---|---|---|
| 2026-11-23 | Module 0 made mandatory; OOP/SOLID and SQL essentials added | Under 1 year of experience; junior interviews weigh C#/OOP fundamentals heavily, and EF Core needs SQL |
| 2026-11-23 | Modules 6-7 (EF advanced, production) targeted at "explain and spot the problem" depth; mock interviews after Modules 2, 6 and the capstone | Goal is interview prep at junior/mid level |
| 2026-11-23 | Added Module 3: Frontend (TypeScript + Angular, React comparison); MVC, EF Core and later modules renumbered 4-7; capstone becomes full-stack | Target role is full-stack Software Engineer; Angular chosen as primary |
| 2026-11-23 | Kept MVC and production modules at full depth; estimated length ~15 weeks | Deadline is tentative; learner prioritises learning depth over speed |

## Session log
| Date | Covered | Results | Next steps |
|---|---|---|---|
| 2026-11-23 | Agreed scope and roadmap; captured goal (interview prep), experience (<1 year), time (5-10 h/week); set up repo and CLAUDE.md; captured role (full-stack SE), tentative 3-month timeframe, Angular as primary frontend; added frontend module | No assessed work yet | — |
| 2026-11-23 | Captured IDE (Visual Studio) and database (SQL Server); ran 5-question diagnostic | 3 solid, 2 not yet; gaps in async and EF query execution; 21 XP | Start M0-T01 (fast pace on basics); give extra weight to M0-T04 and M0-T05 |

## Self-reported (unverified)
| Date | Claim | Status |
|---|---|---|
| 2026-11-23 | Under 1 year hands-on .NET experience | Context only, no credit |

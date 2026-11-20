# Occ Spec DSD Yr 2 — Learning plan

**Goal:** walk into Task 1 on **Tue 9 March 2027** able to do every marked skill without help — Distinction standard.
**Time:** ~1 hr 30 per session (planned total ≈ 60 hrs over 40 sessions, average 91 mins). Evenings after college, **Tuesday, Wednesday and Friday only** (works late Mon and Thu; no weekends), ~1 hour each. Rest/catch-up days and a two-week Christmas break are built in.
**Day-by-day schedule:** the "Daily schedule" tab of the Learning Plan sheet — https://claude.ai/artifact/GfsJi25JqVVjFyuV1D1fLg (40 timed sessions + rest days, 24 Nov 2026 → 5 Mar 2027, each with a minute-by-minute plan and a tick box). The **Spec coverage** tab maps every specification content area (1.1–8.4) to the session that teaches it and where it's marked. Sessions on Tue 29 and Wed 30 Dec are the only ones over Christmas; drop them if needed and the plan slides by two sessions. The week headings below are the original outline; the sheet is the live schedule.
**Practice brief:** use **Netheret IT Support** (Gen 2 AdSAM) as the running practice project, so each unit builds on the last. Use **Rolsa Technologies** (Gen 1, 2025) for the full mock in week 14.
**Progress:** tracked in `learning/progress.md`.

## How every unit works

1. **Learn** — short explanation + one worked example on a *different* brief (ToKa or Rolsa).
2. **Do** — Jamie produces the piece himself for Netheret.
3. **Check** — mark it against `notes/mark-scheme-by-task.md` and `notes/what-gets-a-distinction.md`: which band, what's holding it back, one fix per trait.
4. **Fix** — redo the weakest part.
5. **Recall** — 5 quick questions at the start of the next session on the previous unit.

A unit is **done** when Jamie can produce the piece without notes to at least the top-but-one band, and explain why each choice was made.

---

## Phase 1 — Foundations (weeks 1–2)

### Week 1 · 23–29 Nov — The big picture and the brief
| # | Unit | Done when Jamie can… |
|---|---|---|
| 0 | **How the Occ Spec works** — 3 tasks, 144 marks, what's handed in, **exact AI rules** (`notes/ai-rules.md`), how Task 1 feeds Task 3 | Explain the whole flow from memory and name what's handed in for each task |
| 1 | **Reading a brief** — pull out client, users, needs, features; spot what's implied but not said | Turn the Netheret brief into a stakeholder/needs table in 15 minutes |
| 2 | **SDLC and methodologies** — Waterfall, Agile/Scrum, RAD, Lean, UCD; team roles | Pick a methodology for Netheret and justify it in 3 sentences |

### Week 2 · 30 Nov–6 Dec — Research and decomposition
| # | Unit | Done when… |
|---|---|---|
| 3 | **Sector research** — current practice, emerging tech, judging sources (author, bias, evidence, currency) | Produces a 1-page research appendix for Netheret with 5 rated sources |
| 4 | **Decomposition** — top-down breakdown, then one sub-system to inputs/processes/outputs | Draws a full decomposition diagram covering every Netheret need |

## Phase 2 — Task 1 skills (weeks 3–7)

### Week 3 · 7–13 Dec — Requirements
| # | Unit | Done when… |
|---|---|---|
| 5 | **Functional and non-functional requirements** — specific, measurable, IDs, MoSCoW; *apply, don't define* | Writes 10 FRs + 6 NFRs for Netheret, all testable |
| 6 | **KPIs and user acceptance criteria** — Given/When/Then, linked to requirements | Every FR has a UAC; 5 KPIs with targets and how measured |

### Week 4 · 14–20 Dec — Risk, law and justification
| # | Unit | Done when… |
|---|---|---|
| 7 | **Security risks** — SQL injection, XSS, MITM, weak auth, data breach; likelihood × impact; mitigation and contingency; CIA | Risk table for Netheret with 6 risks, each mitigated |
| 8 | **Legal and standards** — UK GDPR/DPA 2018, Computer Misuse Act, CDPA 1988, Equality Act, PECR, W3C/WCAG, ISO/IEC/IEEE 90003 | Says how each law applies to *Netheret specifically* and how the solution handles it |
| 9 | **Writing the justification** — linking needs → solution → risks → law; technical vs client language | Writes a 1-page justification section and gets it to the top band |

### Week 5 · 21 Dec–3 Jan — 🎄 Light week
- One session: recall quiz on units 0–9.
- Optional: read the 2023 Distinction exemplar (`papers/gen1/exemplars/`) and note 5 things it does that you don't yet.

### Week 6 · 4–10 Jan — Data design
| # | Unit | Done when… |
|---|---|---|
| 10 | **ERDs** — entities, attributes, keys, crow's foot, resolving many-to-many | Draws a Netheret ERD (6+ entities) from the brief alone |
| 11 | **Normalisation to 3NF** | Normalises a messy ticket spreadsheet to 3NF and explains each step |
| 12 | **Data dictionary and validation** — types, sizes, formats, ranges, examples, input masks, error messages | Full dictionary matching the ERD exactly, consistent naming |

### Week 7 · 11–17 Jan — Interface design
| # | Unit | Done when… |
|---|---|---|
| 13 | **UX/UI principles** — layout, white space, visual hierarchy, conventions, cognitive load, accessibility | Critiques 3 real sites using the mark scheme words |
| 14 | **Style guide** — colours (with contrast), fonts and sizes, spacing, components, accessibility options | Netheret style guide on one page |
| 15 | **Wireframes** — desktop + mobile for key screens; detailed enough for a third-party developer | 4 key Netheret screens, desktop + mobile |

## Phase 3 — AI and build skills (weeks 8–11)

### Week 8 · 18–24 Jan — The AI log
| # | Unit | Done when… |
|---|---|---|
| 16 | **Choosing problems** — 5 problems across front end and back end, 2+ languages, linked to the solution | Picks 5 Netheret problems and justifies each |
| 17 | **Prompting and reviewing** — precise narrow prompts; specific positives/negatives; refine; integrate | Full AI log for 2 problems, review section at top band |

### Week 9 · 25–31 Jan — Stack and architecture
| # | Unit | Done when… |
|---|---|---|
| 18 | **Choosing the stack** — 2 permitted languages, front/back end, API, database; Docker + SQLite fallback | **Decides the stack** and records it in `claude/notes/working-notes.md` |
| 19 | **Project structure and Git** — folders, classes, config, GitHub Flow, commit messages | Sets up a clean starter project in the chosen stack |

### Week 10 · 1–7 Feb — Core build skills
| # | Unit | Done when… |
|---|---|---|
| 20 | **Database from the ERD** — DDL, seed data, parameterised queries, CRUD | Builds the Netheret DB and does CRUD on tickets |
| 21 | **Secure login and roles** — hashing + salting, sessions, role-based access, 2FA idea | Working login with 3 roles, no plain-text passwords |
| 22a | **Debugging with AI the allowed way** — exact error + smallest code + expected result; ask *why*; log it in the source and test logs | Fixes 3 real bugs with AI and logs each correctly |
| 22 | **Front end ↔ back end** — forms, validation both sides, API/JSON, error messages | A ticket form that validates and saves through the API |

### Week 11 · 8–14 Feb — The features every brief asks for
| # | Unit | Done when… |
|---|---|---|
| 23 | **Accessibility panel** — font size, contrast, saved per user; alt text; keyboard nav; W3C validator | Panel that saves preferences and passes the validator |
| 24 | **Dashboard / calculator / scheduling** — a chart from DB data; a clash-free booking check | One chart + one scheduling rule working |
| 25 | **Legal features** — cookie notice, privacy policy, T&Cs, consent | All three in the prototype |

## Phase 4 — Prove it and evaluate it (weeks 12–13)

### Week 12 · 15–21 Feb — Testing and logs
| # | Unit | Done when… |
|---|---|---|
| 26 | **Testing** — unit tests (xUnit/pytest/PHPUnit), integration, security, load, compatibility; normal/extreme/erroneous data; regression | 15-row test log with automated test screenshots and fix → retest |
| 27 | **Change log and source log** — dated, versioned, not a narrative; AI/third-party code, assets, licences, IP | Both logs filled for the practice build |
| 28 | **Packaging and screencast** — build + read-me; narrated front and back end demo | 3-minute narrated screencast |

### Week 13 · 22–28 Feb — Feedback and evaluation
| # | Unit | Done when… |
|---|---|---|
| 29 | **Feedback materials** — questionnaires (open + closed), observation, paired code review, technical vs non-technical | Feedback pack for the practice build |
| 30 | **Analysing feedback** — tables, charts, deciding what to change | Turns 5 fake responses into charts + 3 actions |
| 32 | **Change, maintenance and user support** — drivers of change, change management, release notes, user guide/FAQ, issue resolution (spec 8.1–8.4, PO3 18 marks) | Writes release notes + FAQ and explains the issue-resolution process |
| 31 | **Evaluation under task conditions** — assets and sources, each requirement met/partly/not, further development backed by quotes | Writes an evaluation in **2.5 hours, no internet, no AI** |

## Phase 5 — Mock and ready (week 14–15)

### Week 14 · 1–7 Mar — Timed Task 1 mock
- **Rolsa Technologies** (Gen 1, 2025) brief, Gen 2 format: proposal + designs + AI log under time limits (scaled: ~6 hrs total over the week).
- Mark it against the Gen 2 mark scheme. Fix the two weakest traits.
- Confirm with college: tools, languages, Docker, Task 3 date, whether research notes can be brought in.

### Mon 8 Mar — Ready check
- Recall quiz across all units.
- Checklist `checklists/task-checklists.md` read through once.
- Then: **from 9 March, AI help stops except where the task booklet allows.**

---

## Fast reference: unit → mark scheme

| Units | Task / marks |
|---|---|
| 1–9 | Task 1A Proposal (24) + Quality of communication (6) |
| 10–15 | Task 1B Designs (12) |
| 16–17 | Task 1C AI log (12) |
| 18–25 | Task 2A Prototype (30) |
| 26–28 | Task 2B Documentation (18) |
| 29–30 | Task 3A Feedback (24) |
| 31 | Task 3B Evaluation (18) |

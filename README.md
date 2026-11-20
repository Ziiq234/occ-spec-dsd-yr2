# Occ Spec DSD Yr 2

Prep for my **T Level Digital Software Development (Gen 2) Occupational Specialism**: three supervised **tasks**, March–May 2027, 144 marks. **Aim: Distinction.**

> ⚠️ Keep this repo **private**. The past papers in `papers/` are Pearson / DfE copyright, here for personal study only.

## Key dates (2027)

| Task | Dates | Time | Marks |
|---|---|---|---|
| **Task 1** – Analyse the problem and design a solution | Tue 9 Mar → Fri 19 Mar | 18 hrs | 54 |
| **Task 2** – Develop the solution | Mon 22 Mar → Fri 23 Apr | 20 hrs | 48 |
| **Task 3** – Gather feedback (3a) and evaluate (3b) | Sat 24 Apr* → Wed 5 May | 12.5 hrs | 42 |

\* 24 Apr is a Saturday — check with college whether it's Mon 26 Apr.

## Start here

1. **[`learning/`](learning)** — the learning plan, schedule, progress and practice work. Sessions are Tue/Wed/Fri evenings, ~1 hr 30. Live schedule: [Learning Plan sheet](https://claude.ai/artifact/GfsJi25JqVVjFyuV1D1fLg).
2. **[`notes/ai-rules.md`](notes/ai-rules.md)** — exactly where AI is and isn't allowed.
3. **[`notes/what-gets-a-distinction.md`](notes/what-gets-a-distinction.md)** — what examiners reward and what lost marks.
4. **[`HANDOFF.md`](HANDOFF.md)** — one-page summary of everything; paste into any new Claude chat.

## How the repo is organised

```
occ-spec-dsd-yr2/
├── README.md              ← you are here
├── HANDOFF.md             ← full summary for any new chat
├── CLAUDE.md              ← rules Claude follows in this repo
│
├── learning/              ← MY LEARNING — plan, schedule, progress, sessions, practice
│   ├── learning-plan.md       units 0–32 and what "done" looks like
│   ├── daily-schedule.csv     40 timed sessions (backup of the sheet)
│   ├── spec-coverage.md       spec 1.1–8.4 → units → where it's marked
│   ├── progress.md            status + confidence tracker
│   ├── sessions/              one note per session
│   └── practice/              my practice work, one folder per unit
│
├── notes/                 ← WHAT I NEED TO KNOW — written summaries
│   ├── ai-rules.md                  exact AI rules per task
│   ├── what-gets-a-distinction.md   lessons from graded exemplars + examiner reports
│   ├── mark-scheme-by-task.md       Gen 2 marks, task by task
│   ├── specification-summary.md     the spec, Gen 1 vs Gen 2, grade boundaries
│   ├── past-briefs-and-patterns.md  every past client and what they keep asking for
│   ├── lessons-from-past-project.md Archie's 2023 Pass project reviewed
│   └── database-plan.md             Docker database + SQLite fallback
│
├── papers/                ← SOURCE MATERIAL — official papers (read-only)
│   ├── gen2/   SAM (ToKa Fitness) + AdSAM (Netheret): booklets, mark schemes, log templates
│   └── gen1/   2022 GibJohn, 2023 Health Advice, 2025 Rolsa; Pass + Distinction exemplars; examiner reports
│               (each has a text/ folder of plain-text copies for searching)
│
├── templates/             ← STARTERS — requirements, data dictionary, style guide, AI log, test log, change/source log, file names
├── checklists/            ← TICK-LISTS — one per task, from the mark scheme
├── docker/                ← PRACTICE DATABASE — docker-compose for SQL Server / PostgreSQL
│
└── claude/                ← CLAUDE'S SPACE — working notes, session log, skills
    ├── notes/
    └── skills/occ-spec-tutor/
```

## The one thing to remember

The **requirements, KPIs and acceptance criteria written in Task 1** are what Task 3 is marked against. Make them specific and measurable in March, or they cost marks again in May.

## To do

- [x] Gen 2 and Gen 1 past papers, exemplars and examiner reports
- [x] Learning plan, timed schedule, spec coverage, tutor skill
- [ ] Confirm with college: AI tool provided, languages/IDEs, design tools, Docker on college PCs, Task 3 start date, whether research notes can be brought in
- [ ] First session: Tue 24 Nov — how the Occ Spec works + reading a brief

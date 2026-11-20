# Occ Spec DSD Yr 2 — Handoff / Reference

**Student:** Jamie Jones · **Qualification:** T Level Technical Qualification in Digital Software Development (Pearson, Gen 2) · **Written:** 20 Nov 2026

Use this file to brief any future session on everything worked out so far. Call it **Occ Spec DSD Yr 2**. It is a set of supervised **tasks**, not an exam.

---

## 1. Key dates (2027)

| Task | Starts | Ends | Time allowed | Marks |
|---|---|---|---|---|
| Task 1 – Analyse and design | Tue 9 Mar | Fri 19 Mar | 18 hrs | 54 |
| Task 2 – Develop the prototype | Mon 22 Mar | Fri 23 Apr | 20 hrs | 48 |
| Task 3 – Gather feedback (3a, 10 hrs) and evaluate (3b, 2.5 hrs) | Sat 24 Apr* | Wed 5 May | 12.5 hrs | 42 |

\* 24 Apr 2027 is a Saturday. Check with college whether it should be Mon 26 Apr.

**Total:** 144 marks, about 50.5 supervised hours, set and marked externally by Pearson, submitted as an electronic portfolio. Worth 50% of the whole T Level.

---

## 2. Qualification facts (from the Gen 2 specification)

- **Gen 1** = Digital Production, Design and Development (2020–2024 cohorts). **Gen 2** = Digital Software Development (2025–2029 cohorts). It's the same T Level, renamed.
- **Grades:** Pass / Merit / Distinction / Unclassified. A T Level needs at least an E in the Core and a Pass in the Occ Spec. A Distinction* overall needs an A* in the Core and a Distinction in the Occ Spec.
- **Permitted languages (at least two):** Python 3 (3.10+), C#, SQL, JavaScript, PHP. This is a fixed list.
- **Internet:** allowed in all tasks except 3b.
- **AI rules:**
  - Task 1: AI is allowed **only** in Activity C, where it is *required* for code snippets (maximum 5 problems, not a whole solution).
  - Task 2: AI is allowed for small code snippets and for testing/debugging only.
  - Task 3: no AI at all. 3b also has no internet.

### Marks by performance outcome
| PO | Area | Marks |
|---|---|---|
| PO2 | Design, implement and test | 57 |
| PO1 | Requirements | 24 |
| PO3 | Change, maintain and support | 18 |
| PO5 | Reliable sources | 18 |
| PO6 | Ethics and risk | 18 |
| PO4 | Collaboration | 9 |

### Gen 1 vs Gen 2
| | Gen 1 | Gen 2 |
|---|---|---|
| Time | 67 hrs | 50.5 hrs |
| Marks | 145 | 144 |
| Languages | Provider chooses | Fixed list of 5 |
| AI | Not part of the assessment | Required in 1C |
| Sources / Ethics marks | 13 / 10 | 18 / 18 |

### Grade boundaries (for reference only — Gen 2 not yet published)
Gen 1, summer 2024, out of 145: **Distinction 99 (~68%) · Merit 68 (~47%) · Pass 38 (~26%)**.

### Specification content to know
- **Design:** wireframes, style guides, clickable prototypes; flowcharts and pseudocode; data dictionary, ERD, 3NF; OOP/TDD/BDD; gitFlow/GitHub Flow.
- **Implementation:** front end and back end in 2+ languages; APIs; packaging; CI/CD stages; coding conventions; 12-factor principles; API/JDBC/ODBC; deployment.
- **Testing:** unit, smoke, integration, system; availability, compatibility, configuration, load; front-end and security testing; acceptance, alpha, beta, closed-box/open-box; valid, invalid, extreme and erroneous test data.
- **Legal/ethics:** IP, copyright, data protection (GDPR), consumer protection, equality, security, licensing; ISO/IEC/IEEE 90003:2018 and W3C.
- **Risk:** likelihood vs seriousness, mitigation, contingency, CIA, backups, business continuity, disaster recovery.
- **Planning:** SDLC, user stories, ERDs, activity diagrams, KPIs, acceptance criteria; Agile, Scaled Agile, Waterfall, RAD, Lean, UCD; secure by design.
- **Sources:** judge by author reputation, bias, evidence, cross-referencing and how current they are.

---

## 3. Past papers (Gen 2) — what they show

Location: OneDrive (Chichester College Group) → `!Classes\exams\`
- `Digital Software Development SAM OS` — SAM, client **ToKa Fitness** (gym: free/paid content, sight-loss accessibility, social features, custom workout and eating plans).
- `DSD OS AdSAM` — Additional SAM (Feb 2026), client **Netheret IT Support Solutions** (IT help desk Tier 1–3: log and manage tickets, schedule on-site jobs, performance insights, knowledge base, job tracking, accessibility, custom schedules for Tier 2/3).
- Each contains the task booklets for Tasks 1–3, a mark scheme and Word templates (AI Log, Test Log, Change and Source Log).

**Both papers are word-for-word the same structure; only the client changes.** Expect the real paper to follow the same layout.

### Task 1 – Analyse and design (54)
- **A Proposal (24, about 9 hrs):** business context; functional and non-functional requirements; decomposition; KPIs and user acceptance criteria; solution description; justification of needs, risks and legal/regulatory points; research appendix.
  - Marking: decomposition 9 · wider issues/justification 9 · requirements/acceptance criteria 6.
  - The mark scheme looks for risks such as SQL injection, XSS, man-in-the-middle (HTTPS/SSL) and input validation; GDPR, W3C, copyright/IP; authorised access only; current practice and emerging tech in the sector.
  - Requirements must be **specific and measurable**, in tables.
- **B Designs (12, about 4.5 hrs):** interface 6 (layout and white space, visual hierarchy, conventions, desktop and mobile, style guide) + data 6 (ERD and data dictionary, data types, validation rules/input masks/error messages, consistent naming).
- **C AI log (12, about 4.5 hrs):** problem choice 3 · prompts 3 · **output review 6**. Cover up to 5 problems across the front end and back end, in more than one language; refine prompts each time; give specific positives and negatives and the refinements needed.
- **Quality of communication (6)** across all of Task 1.
- File names: `Task1_Proposal_[RegNo]_[Surname]_[Initial]`, `Task1_DesignDocs_[Doc]_…`, `Task1_AILog_…` (PDF; add _01, _02 for multiple files).

### Task 2 – Develop (48)
- **A Prototype (30, about 12.5 hrs):** functionality 8 · code organisation 8 · user experience 8 · legal/regulatory 6.
  - 2+ languages, front end and back end, a linked multi-table database, modular code (functions/classes), comments, constants, few globals, defensive programming, exception handling, validation and sanitisation, clear error messages, accessibility options (font size and colours), cookie notice, GDPR, privacy policy, T&Cs, CIA security controls.
- **B Documentation (18, about 7.5 hrs):** suitability of testing 6 · testing driving improvements 3 · use of others' content (source log) 6 · change log 3.
  - Include automated tests (unit, load, validation) **with screenshots of the setup and results**, AI-assisted testing, and manual/black-box/compatibility testing.
  - Change log = date + short summary + file name and version. **Not** a step-by-step narrative.
  - Source log = source/URL, original content, how it was used/adapted, IP/legal points (including AI-generated content).
- **Hand in:** working build, source code, a **screencast** of the front end and back end, the test log and the change/source log.

### Task 3 – Feedback and evaluation (42)
- **3a Feedback (24, 10 hrs, internet allowed):** materials 12 · tools 6 · communication 6. Separate technical and non-technical audiences; questionnaires (open and closed questions), screencasts, observation (pain points), paired code review.
- **3b Evaluation (18, 2.5 hrs, no internet, no AI):** assets and content 6 (why chosen/rejected, validity and reliability of sources, bias, legal/ethical) · meets requirements and acceptance criteria 3 · further development 6 (backed by feedback quotes and examples).
- **The requirements and acceptance criteria written in Task 1 are what Task 3 is marked against. If they're vague in March, it costs marks again in May.**

---

## 4. Reference project — Archie Paice, 2023 (Gen 1), graded **Pass**

- Repo: https://github.com/archie-paice/Invisible-Ink (code only, no documentation). C#/WPF booking system for a piercing studio, SQLite/SQL.
- Jamie's view: the standard is much higher now because AI is allowed.
- **Why it only passed:** six near-identical window files, one per staff member (copy-paste); a login that's an if/else chain on names; plain-text passwords that are never checked; a search query open to SQL injection; health data and dates of birth stored with no GDPR measures; a database with no proper links (names stored as text); leftover joke names and comments (`New_Task_Lab_Wars`, `LoserInfo`); really only C# with some SQL.
- **Good points:** mostly parameterised queries, some try/catch, real business rules (availability, 3 per time slot, 9–5 hours).
- **How to beat it:** reusable role-based screens; hashed passwords and role-based access; parameterised SQL everywhere; a linked, normalised database built from the ERD; a clear second language (e.g. a JS web front end with a C# or Python API); consistent naming and useful comments; unit tests; GDPR and accessibility built in.

---

## 5. Decisions and ideas so far

- **Database:** Archie suggested running the DB in **Docker** (e.g. SQL Server, MySQL or PostgreSQL) instead of phpMyAdmin or a full SQL Server install, which bogs down the main PC.
  - Don't auto-start Docker Desktop; run `docker compose down` when finished; cap WSL memory in `C:\Users\<you>\.wslconfig` (`[wsl2]` / `memory=4GB`). PostgreSQL/MySQL are lighter than SQL Server.
  - **Check whether college PCs allow Docker** (it needs admin rights and WSL2/Hyper-V).
  - Plan: support both SQL Server (Docker) and **SQLite**, switched by connection string, so the marker can run it with nothing installed. Fallback code is credited in the mark scheme.
- **Designs:** will need ERDs and the full design set, aiming for top-band, really good design. Not started yet.
- **Languages known:** C#, Python, SQL (all on the permitted list), plus some C++.

## 6. Preferences for future sessions

- Focus on the Occ Spec tasks only; **don't bring in the NHS placement**.
- Call them **tasks**, not an exam.
- Jamie asked for everything about the Occ Spec to be remembered.

## 7. Still to do

- [ ] Share the **Gen 1** past papers (Digital Production, Design and Development).
- [ ] Confirm with college: allowed languages/IDEs, design tools (draw.io / Figma / Lucidchart?), hosting, Docker on college PCs, and the Task 3 start date.
- [ ] Practise ERDs, data dictionaries, wireframes and a style guide (on the Netheret or ToKa brief).
- [ ] Practise an AI log (prompts, then a critical review, then refinement).
- [ ] Set up a Docker DB at home with a SQLite fallback.
- [ ] Optional: a weekly prep plan up to 9 March.

## 8. Sources

- Pearson Gen 2 specification: https://qualifications.pearson.com/content/dam/pdf/TLevels/digital-software-development/2025/specification-and-sample-assessment-materials/digital-dsd-specification.pdf
- Pearson Gen 1 → Gen 2 names (Sept 2025 update): https://qualifications.pearson.com/en/news-policy/subject-updates/ict/t-level-sep25-update.html
- Pearson Gen 1 (DPDD) specification, 2020: https://qualifications.pearson.com/content/dam/pdf/downloads/digital-webinar/T-Level_Specification.pdf
- Pearson grade boundaries, summer 2024: https://qualifications.pearson.com/content/dam/pdf/Support/Grade-boundaries/t-levels/t-level-grade-boundaries-summer-2024.pdf
- Skills England: https://skillsengland.education.gov.uk/qualifications/TL0006a
- Research doc: https://claude.ai/artifact/VDVWhnZ2MCrRWJzobVTwSo

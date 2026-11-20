# What gets a Distinction — lessons from Gen 1 exemplars and examiner reports

Sources (all in `papers/gen1/`):
- Lead examiner reports 2022 and 2023 (`examiner-reports/`)
- Graded exemplar portfolios with examiner commentary: 2022 GibJohn **Pass** and **Distinction**, 2023 Health Advice Group **Pass** and **Distinction** (`exemplars/`)
- Admin support guide 2024 (`admin/`)

Gen 1 is the older version of the same qualification. Gen 2 swaps the algorithm designs and test strategy in Task 1 for the AI log, and adds the change/source log, but the proposal, designs, prototype, testing, feedback and evaluation are marked on the same traits. These lessons carry straight over.

## How students actually did (Gen 1)
- 2023: 145 marks available. Lowest 0, highest 128, **mean 70.1**. 2022 mean was 72.6.
- 2024 boundaries: Distinction 99, Merit 68, Pass 38.
- So the average student lands around a Merit. A Distinction needs ~30 marks more than average.

## The biggest single lesson
**Apply, don't define.** Both examiner reports say the proposal "should not explain what functional requirements are or define the legislation". The 2023 Pass student lost marks for writing *what a KPI is* and *what user acceptance criteria are* instead of writing the actual KPIs and criteria for the client. Every sentence should be about *this* client.

## The Distinction prototype wasn't finished
The 2023 Distinction student (HTML/CSS + PHP + MySQL, weather API) **ran out of time**: no admin page, the accessibility panel didn't save, articles weren't loaded from the database, policy and T&Cs pages were placeholders. They said so honestly in the development documentation and still got a Distinction.

→ Marks come from the **whole portfolio**: designs, documentation, testing, feedback and evaluation. A smaller, well-built, well-documented prototype beats a big half-broken one. Don't sink all of Task 2 into features.

The 2022 Distinction student used Python (Django) + HTML/CSS/JS + SQLite.

## Task by task — Distinction vs Pass

### Proposal
| Distinction | Pass |
|---|---|
| Every requirement tied to the scenario, **with a justification for each** | Basic definitions of requirement types |
| KPIs that are real metrics for this client (e.g. engagement with advice, data accuracy, retention) | Explains what a KPI *is* |
| Acceptance criteria with justification of how they show the project objectives are met | Explains what acceptance criteria *are* |
| Risks named **and** linked to the legal side of the scenario, with mitigation | Risk mitigation "present but needs more profound elaboration" |
| Considers wider issues and how things connect | "Needs more in-depth reasoning and detail" |

### Interface designs
- Distinction: clear zones, deliberate line spacing, related items grouped, information in chunks, **responsive layouts for mobile and desktop**, sizing that guides attention, nav order that shows a route through the info, standard icons.
- Must state **background colours, text sizes, fonts** — "how would the web developer build the website without knowing text sizes, colours and other descriptive features?"
- Weak: poor visuals, ignores conventions, missing specs.

### Data design
- Distinction: data dictionary with **data type, size, format, valid values/range, example** for every field; data flow diagram; ERD; consistent naming; error handling that guides the user to fix the problem.
- Pass: "naming conventions mostly appropriate but inconsistent"; error handling "only covers some of the inputs/processes".

### Decomposition / algorithms
- Show the **whole breakdown first** (diagram / stepwise refinement), then take one sub-system down to pseudocode or a flowchart.
- Distinction identified all inputs, processes, outputs (including error messages and notifications).
- Pass: "think about useful algorithms other than the standard ones, like log-in or registration forms."
- Gen 2 note: algorithm designs aren't a separate Task 1 item any more, but the proposal still marks **decomposition (9 marks)**, and flowcharts/pseudocode are in the spec.

### Prototype (Task 2)
- Two languages; most popular were **Python, PHP, JS and SQL**.
- **Justify** approaches — comments in the code explaining *why*, not just what.
- Provide a **packaged build with a read-me**, or a **narrated** video. Examiners actually ran the Distinction student's build.
- Legal/regulatory: show it works in **different browsers**; **validate HTML/CSS with the W3C validator**; usernames and passwords, **cookie notice, two-factor authentication**.
- Weak: describes what happened instead of justifying; no comments; linear code; lots of errors.

### Testing
- Distinction: tests inputs, calculations, validation and processes with **normal, erroneous and extreme** data; records what was found and how it was fixed; **regression testing**; clear test → fix → retest cycle.
- Weak: relied on the IDE to catch syntax errors and stopped there.
- Examiner advice: test against the **requirements**, try different validation/verification methods, regression test, use all three data types.

### Feedback (Task 3a)
- Use **at least two different techniques** (e.g. survey + observation).
- Questions aimed separately at **technical and non-technical** testers.
- Questions designed so the answers can actually improve the product.
- **Visualise and analyse** the results (charts, tables) — "a detailed visualisation of the data gathered and analysed".
- The 2023 Distinction student's questionnaire had a star-rating question set up as a text box and noted it as a flaw — check your forms before sending.

### Evaluation (Task 3b)
- Assets: where they came from, how valid and reliable the source is, copyright/licence, **why** each was chosen and how it helps the user.
- Evaluate against **functional and non-functional requirements, KPIs and acceptance criteria**.
- "On the threshold of distinction, the evaluations often needed … to consider the user's needs effectively." → **Keep user needs front and centre.**
- Pass: cursory source checks, few examples, feedback barely used, simplistic future-development rationale.

## Rules from the admin guide worth knowing
- All tasks are supervised, medium control; work stays on college systems.
- Internet may be used for research, assets, small code snippets, docs/forums and public datasets — **not** to download complete solutions.
- Every asset and code snippet (including AI) must be logged: source, what it is, purpose, **date and where retrieved**.
- Gen 1 allowed research notes outside sessions, but only **facts and figures**, no interpretation of the scenario, and they get submitted as an appendix. Check whether Gen 2 has the same rule.
- No further changes once a task window closes. Tasks 1 and 2 are read-only in Task 3.

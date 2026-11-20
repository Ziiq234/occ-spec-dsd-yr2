# Mark scheme by task — what gets the top band

Built from the Gen 2 SAM and AdSAM mark schemes (`papers/gen2/*/mark-scheme.pdf`). Marking is **best fit**: examiners pick the band that best matches, then the mark within it depends on how securely *every* trait is shown.

The two papers are identical apart from the client:
- **SAM** — ToKa Fitness (gym: info and advice, free/paid content, sight-loss accessibility, social features, custom workout and eating plans)
- **AdSAM** — Netheret IT Support Solutions (help desk Tier 1–3: log/manage tickets, schedule on-site jobs, performance insights, knowledge base, job tracking, accessibility, custom schedules)

---

## Task 1 — Analyse and design (54 marks, 18 hrs)

### Activity A — Proposal (24 marks, ~9 hrs)

| Focus | Marks | Top band needs |
|---|---|---|
| Decomposing the problem | 9 | *Fully* identifies problems, *effective* decomposition; solution fully meets client/user needs, mitigates risks, addresses law/regs |
| Wider issues in context | 9 | *Comprehensive* lines of reasoning that justify needs, risk mitigation and legal/regulatory points |
| Business context | 6 | *Comprehensive and perceptive* definitions of functional reqs, non-functional reqs, user acceptance criteria |

Include: business context · functional and non-functional requirements · decomposition · KPIs and user acceptance criteria · solution description · justification (needs, risks, law) · research appendix.

The mark scheme specifically looks for:
- **Risks + fixes:** malicious input → validation; man-in-the-middle → SSL/HTTPS/encryption; XSS → content security policy and sanitisation; SQL injection → sanitised/parameterised input.
- **Wider issues:** privacy, user support, feedback on user errors, payment details, sensitive client data, accuracy of advice, copyright/IP of third-party code and APIs, right level of technical detail per user, authorised access only, W3C and professional bodies.
- **Research:** current practice and emerging tech in the client's sector (e.g. expert systems, CRM/ticketing, multi-channel support, dashboards, tablets on site).
- **Data handling:** client vs server storage, database type, APIs, emails/notifications.
- **Accessibility:** alt text, resizable fonts, selectable colour schemes, W3C.
- **Justify** design choices with research: conventions, expected features, fixing competitors' complaints, unique features.

### Activity B — Designs (12 marks, ~4.5 hrs)

| Focus | Marks | Top band needs |
|---|---|---|
| Interface design | 6 | *Excellent*, *highly effective* layout and white space, visual hierarchy, common conventions |
| Data design | 6 | Data *fully* appropriate (variables, structures, types); *effective* error handling; *fully consistent* naming |

- **Interface:** clear zones, line spacing (leading), related info grouped, no overload, **desktop and mobile** versions, size/order shows importance, standard icons, nav at top or left, hamburger menu on mobile, consistent fonts/colours/imagery, help and documentation. A **style guide** beats heavy annotation.
- **Data:** ERD (proper relationship notation) **plus** data dictionary; DFDs and other diagrams optional; normalisation if it fits. User account levels, schedules, metrics, customer data, linked records.
- **Error handling:** validation rules, input masks, type casting, error messages, field lengths.

### Activity C — Generative AI (12 marks, ~4.5 hrs)

| Focus | Marks | Top band needs |
|---|---|---|
| Problem solving | 3 | Effective coverage — range of processes linked to other components, more than one language |
| Use of prompts | 3 | Highly precise, concise prompts; narrow scope; refined after each iteration |
| Output review | **6** | Thorough: specific positives *and* negatives, refinements needed, granular |

- Max **5 problems**. Not a whole solution. Code must fit into a bigger solution.
- Good problems: validation (regex phone/email), front-end ↔ back-end data exchange, domain calculations (metrics, scheduling, conflict checks), filtering and charts/dashboards, API or knowledge-base content, password hashing / writing tables.
- Log: prompts, output, review (how well it works, robustness — exceptions, SQL injection), refinements (new prompts, manual edits like renaming variables or adding features).

### Quality of communication (6 marks)

Across all of Task 1. Technical vocabulary used correctly; suits the audience; tables/bullets for measurable requirements with explanation separately; technical detail for developers, plain language when justifying to the client; clear wireframes; style guide; ERD + data dictionary.

### File names
`Task1_Proposal_[RegNo]_[Surname]_[Initial]` · `Task1_DesignDocs_[DocName]_[RegNo]_[Surname]_[Initial]` · `Task1_AILog_[RegNo]_[Surname]_[Initial]` — PDF; add `_01`, `_02` for multiple files.

---

## Task 2 — Develop (48 marks, 20 hrs)

### Activity A — Prototype (30 marks, ~12.5 hrs)

| Focus | Marks | Top band needs |
|---|---|---|
| Functionality | 8 | *Highly efficient* code in 2+ languages, minimal errors, consistently correct outcomes |
| Code organisation | 8 | *Easily* maintainable: consistent naming, logical organisation, informative comments |
| User experience | 8 | *Consistently effective* input handling, guidance/error messages, outputs; *fully robust* |
| Legal and regulatory | 6 | *Effective* accessibility, compatibility, legal/ethical; *fully effective* CIA security controls |

- **Functionality:** two languages (e.g. JS + PHP/SQL, Python + SQL, C# + SQL); linked multi-table database; DML and DDL; functions, procedures, classes; server-side request/response; APIs and JSON/XML parsing; modular. Covers user access (accounts, password changes), data collection and processing, front ↔ back-end exchange, key calculations, filtering and visualisation.
- **Code organisation:** no pages of nested ifs or copy-paste; clear indentation; classes/objects; comments explaining logic; local variables over globals; constants; consistent style; defensive programming; good exception handling.
- **UX:** validation and sanitisation; input masks; useful, usable, desirable, findable; short jargon-free errors that say how to fix the problem; help/labels; fallback code for different platforms.
- **Legal:** selectable accessibility (font size, colours); sensible base colours; compatibility (standalone or web standards); cookie notice; GDPR; privacy policy; IP (see source log); T&Cs; health and safety where relevant.

### Activity B — Documentation (18 marks, ~7.5 hrs)

| Focus | Marks | Top band needs |
|---|---|---|
| Suitability of testing | 6 | Thorough, detailed tests of inputs, calculations, validation, processes |
| Testing → iteration | 3 | Effective iterative development shown |
| Content produced by others | 6 | Comprehensive: how used, legal/ethical, fit to task |
| Change log | 3 | Thorough, detailed records |

- **Testing:** automated tools (performance, stress, load, validation, **unit**) — show the setup **and** results **and** what you'll do about them; AI-assisted testing; manual (visual debugging, black box, paired code review, compatibility). Use a wide range.
- **Iteration:** errors found and fixed; refinements (efficiency, standards, less redundancy); improvements (features, UX, accessibility).
- **Source log:** code snippets, synthetic test data, information content, assets/media — source, original, how integrated, dependencies, legal (proprietary? how was AI content made? IP risk?).
- **Change log:** date + brief summary + file name and version. **Not** a step-by-step story.

### Hand in
Exported/packaged working prototype · source code · **screencast** of front end and back end · `Task2_ChangeSource_log_[RegNo]_[Surname]_[Initial]` · `Task2_TestLog_[RegNo]_[Surname]_[Initial]`.

---

## Task 3 — Feedback and evaluation (42 marks, 12.5 hrs)

### 3a — Gathering feedback (24 marks, 10 hrs, internet allowed)

| Focus | Marks | Top band needs |
|---|---|---|
| Materials | 12 | High-quality feedback on different aspects of the prototype |
| Feedback tools | 6 | Feedback *fully* supports evidence-informed iteration |
| Communication | 6 | Fully effective for technical *and* non-technical audiences |

Screencasts (technical and non-technical versions), questionnaires (open + closed, sections per audience), observation records (pain points; structured/unstructured/participant), paired code review records. Testers: range of ages and abilities, domain professionals, programmers.

### 3b — Evaluation (18 marks, 2.5 hrs, **no internet, no AI**)

| Focus | Marks | Top band needs |
|---|---|---|
| Assets and content | 6 | Comprehensive: appropriateness, validity/reliability of sources, legal/ethical; corroborated across sources |
| Evaluation of the solution | 3 | Comprehensive against functional/non-functional reqs and acceptance criteria **from Task 1** |
| Further development | 6 | Comprehensive rationale backed by fully relevant, perceptive examples and feedback |

- Assets: third-party/synthetic data, media, code snippets, realistic info for the scenario; primary vs secondary; up to date; bias.
- Legal/ethical: copyright and IP, GDPR/encryption/privacy policy, representation, accessibility, cookies, T&Cs.
- Use **specific quotes from feedback** and **examples from the prototype**.

### File names
`Task3_Feedback_[DocName]_[RegNo]_[Surname]_[Initial]` · `Task3_Evaluation_[RegNo]_[Surname]_[Initial]` (PDF).

# Change and source log — practice template (Task 2B)

> Real task: use the Pearson Word template.

## Change log
Brief, notable changes only — **not** a step-by-step story.

| Date | Summary of change | File name and version |
|---|---|---|
| 22/03/2027 | Created database schema (5 tables) from ERD | `schema.sql` v1.0 |
| | Fixed SQL injection in search found in test T03 — now parameterised | `TicketRepository.cs` v1.3 |

## Source log
Everything you didn't write yourself: code snippets (including AI), synthetic test data, information content, images, icons, fonts, libraries.

| Source (inc. URL) | Original content | Further information (where used, how adapted, dependencies, legal considerations) |
|---|---|---|
| ChatGPT, prompt 2.3 in AI log | Email validation function | Used in `RegisterForm.js`; renamed variables, added trim and length check. AI output — no licence issue but checked for correctness |
| Font Awesome (fontawesome.com) | Icon set | Free licence (CC BY 4.0 icons); attribution in footer |
| Mockaroo | 200 synthetic customer records | No real personal data → no GDPR issue |

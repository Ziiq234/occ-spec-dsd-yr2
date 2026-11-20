# Lessons from a past project — Archie Paice, 2023 (Gen 1), graded Pass

Repo: <https://github.com/archie-paice/Invisible-Ink> — code only, no documentation.
C# / WPF booking system for a piercing studio with an SQL/SQLite database. Receptionists book appointments and record health checks; each piercer sees their own schedule.

The standard is higher now: AI is allowed, so clean code is the baseline.

## Why it only passed

| Problem | Mark scheme area hit |
|---|---|
| Six near-identical window files, one per staff member (~167 lines each, only the name differs) | Code organisation — copy-pasted procedural code |
| Login is a long if/else chain on staff names | Code organisation, maintainability |
| Leftover names/comments: namespace `New_Task_Lab_Wars`, class `ClasLos`, variable `LoserInfo`, "our DB :)" | Code organisation — naming, commenting |
| Passwords stored in plain text and never checked (login asks for user ID only) | Legal/regulatory — CIA security controls |
| Client search builds SQL from user input: `LIKE '%{searchText}%'` | Security — SQL injection |
| Health check data and DOB stored with no consent/privacy/access control | Legal — GDPR special category data |
| Bookings store client/staff names as text, no foreign keys; dates stored as text | Functionality — data model |
| Really one language (C#) plus some SQL | Functionality — 2+ languages |

## What it did well
- Most queries parameterised.
- Some try/catch error handling.
- Real business rules: staff availability by day, max 3 appointments per slot, 9–5 working hours.
- Simple, working UI.

## How to beat it
- One reusable screen per **role**, taking the user as a parameter.
- Hashed + salted passwords, role-based access.
- Parameterised SQL everywhere.
- Normalised, linked database built straight from the ERD.
- A clear second language (e.g. JS web front end + C# or Python API, with SQL).
- Consistent naming, comments that explain *why*.
- Unit tests with evidence.
- GDPR, accessibility, cookie notice, privacy policy built into the app.
- Full documentation (the part that was missing entirely).

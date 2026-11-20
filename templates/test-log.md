# Test log — practice template (Task 2B)

> Real task: use the Pearson Word template. Show **automated test setup and results**, and what you did about failures.

| # | Description of test (purpose, tool, data) | Type | Test data (valid / invalid / extreme / erroneous) | Expected outcome | Actual outcome | Comments and intended actions |
|---|---|---|---|---|---|---|
| T01 | Email validation rejects missing "@" — xUnit/pytest unit test | Unit | `acme.co.uk` (invalid) | Returns false, error message shown | | |
| T02 | Login with correct details | Black box | Valid user | Redirect to dashboard for that role | | |
| T03 | SQL injection in search box | Security | `' OR 1=1 --` (erroneous) | Treated as text, no extra rows | | |
| T04 | 100 concurrent requests to ticket list API | Load | — | < 2s average response | | |
| T05 | Text size 150% on mobile | Compatibility / accessibility | — | No overlap, all content usable | | |

## Test types to cover
- Unit, integration, system, smoke
- Validation (valid / invalid / extreme / erroneous)
- Security (injection, XSS, access control)
- Load / performance / stress
- Compatibility (browsers, screen sizes, OS)
- Accessibility (contrast checker, keyboard only, screen reader)
- AI-assisted code review
- Paired code review

# Requirements, KPIs and acceptance criteria — template

> Make every line **specific and measurable**. Task 3B evaluates the prototype against these.

## Functional requirements

| ID | Requirement | User(s) | Priority (MoSCoW) | How it will be tested |
|---|---|---|---|---|
| FR01 | The system shall let a Tier 1 user log a new support ticket with company, contact, category, priority and description | Tier 1 | Must | Create ticket with valid data → saved with unique ID and timestamp |
| FR02 | | | | |

## Non-functional requirements

| ID | Requirement | Category | Measure |
|---|---|---|---|
| NFR01 | Pages load in under 2 seconds with 50 concurrent users | Performance | Load test result |
| NFR02 | Meets WCAG 2.2 AA (contrast ≥ 4.5:1, keyboard navigable, text resizable to 200%) | Accessibility | Automated + manual check |
| NFR03 | Passwords hashed with a salted algorithm (e.g. bcrypt/PBKDF2); no plain text stored | Security | Code review + DB inspection |
| NFR04 | | | |

## KPIs

| KPI | Target | How measured |
|---|---|---|
| Average time to log a ticket | < 60 seconds | Timed user test |
| | | |

## User acceptance criteria

| ID | Linked req | Given / When / Then |
|---|---|---|
| UAC01 | FR01 | **Given** I am logged in as Tier 1, **when** I submit a ticket with all required fields, **then** I see a confirmation with the ticket number |
| UAC02 | | |

## Decomposition

```
Whole system
├── User accounts and access (roles, login, password reset)
├── Core process (e.g. tickets / bookings)
│   ├── Create
│   ├── Update / track progress
│   └── Close / escalate
├── Scheduling
├── Reporting / dashboard
├── Knowledge base / content
└── Accessibility and settings
```

## Risks

| Risk | Likelihood (1–5) | Impact (1–5) | Score | Mitigation | Contingency |
|---|---|---|---|---|---|
| SQL injection | 3 | 5 | 15 | Parameterised queries, input validation | Restore from backup, patch, audit log |
| Man-in-the-middle | | | | HTTPS/TLS | |
| Cross-site scripting | | | | Output encoding, CSP, sanitisation | |
| Data breach (GDPR) | | | | Role-based access, encryption, minimal data | Breach procedure, ICO within 72 hrs |

## Legal and regulatory

| Law / standard | How it applies | How the solution addresses it |
|---|---|---|
| UK GDPR / Data Protection Act 2018 | | |
| Computer Misuse Act 1990 | | |
| Copyright, Designs and Patents Act 1988 | | |
| Equality Act 2010 / W3C WCAG | | |
| PECR (cookies) | | |
| ISO/IEC/IEEE 90003:2018 | | |

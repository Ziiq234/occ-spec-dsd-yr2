# Data dictionary — template

> Pair this with an ERD that uses proper crow's foot notation. Same names in both.

## Naming conventions
- Tables: `PascalCase`, singular (`Customer`, `SupportTicket`)
- Fields: `PascalCase`, primary keys `<Table>ID`, foreign keys same name as the PK they point to
- Booleans start with `Is`/`Has` (`IsResolved`)
- Dates as `DATE` / `DATETIME`, never text

## Table: `Customer`

| Field | Data type | Size | Key | Required | Validation rule | Input mask / format | Example | Description |
|---|---|---|---|---|---|---|---|---|
| CustomerID | INT | — | PK | Yes | Auto increment | — | 1042 | Unique customer number |
| CompanyName | VARCHAR | 100 | | Yes | Length 2–100, letters/numbers/spaces/&.-' | — | Acme Ltd | Registered company name |
| Email | VARCHAR | 254 | | Yes | Regex email pattern, unique | name@domain.tld | it@acme.co.uk | Main contact email |
| Phone | VARCHAR | 15 | | No | UK format, digits and + only | 00000 000000 | 02392 123456 | Main contact phone |
| CreatedAt | DATETIME | — | | Yes | Default now; not in future | dd/MM/yyyy HH:mm | 20/11/2026 11:40 | When the record was made |

## Error handling summary

| Field | Invalid input | Error message shown to user |
|---|---|---|
| Email | `acme.co.uk` | "Enter an email address like name@company.co.uk" |

## ERD checklist
- [ ] Every entity has a primary key
- [ ] Relationships use crow's foot (1:1, 1:M, M:M resolved with a link table)
- [ ] Foreign keys shown
- [ ] Normalised to 3NF (or a reason given if not)
- [ ] Matches the data dictionary exactly
- [ ] Has a key/legend so a non-technical reader can follow it

# Database plan — Docker with a SQLite fallback

Idea from Archie: run the database in **Docker** instead of phpMyAdmin or a full SQL Server install (which runs Windows services in the background and bogs down the main PC).

## Why
- Start it when coding, stop it after, delete it with nothing left behind.
- The schema and seed data live in code → repeatable, easy to reset for testing, goes in the change log.
- Not stuck with MySQL — can use SQL Server, PostgreSQL or MySQL.
- Professional practice → something to justify in the proposal and the compatibility section.

## Keep Docker light
- Docker Desktop → Settings → turn **off** "Start Docker Desktop when you sign in".
- `docker compose down` (or quit Docker Desktop) when finished.
- Cap WSL2 memory: create `C:\Users\<you>\.wslconfig` (example in `docker/wslconfig.example`).
- SQL Server needs ~2 GB RAM. PostgreSQL/MySQL need a few hundred MB.

## Risks to check
1. **College PCs** — Docker needs admin rights and WSL2/Hyper-V. Ask whether it can be used on the PCs for the supervised tasks.
2. **Submission** — the marker needs to run the prototype. Don't make them install Docker.
3. **Practise it** several times before relying on it.

## Plan
Write the app so it can use either:
- **SQL Server or PostgreSQL in Docker** — main development build, and
- **SQLite** — a single file, nothing to install, used for the packaged submission and if Docker is blocked.

Switch with the connection string (config file or environment variable). The mark scheme credits "fall back" code for different systems.

See `docker/` for a starter `docker-compose.yml`.

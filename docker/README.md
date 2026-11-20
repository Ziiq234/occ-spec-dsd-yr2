# Docker practice database

1. Install Docker Desktop (needs WSL2). Turn off "Start Docker Desktop when you sign in".
2. Copy `.env.example` to `.env` and set your own passwords. `.env` is git-ignored.
3. Optional: copy `wslconfig.example` to `C:\Users\<you>\.wslconfig` to cap memory, then run `wsl --shutdown`.
4. Start one database:
   - SQL Server: `docker compose --profile sqlserver up -d`
   - PostgreSQL (lighter): `docker compose --profile postgres up -d`
5. Connect from VS Code / Azure Data Studio / your app:
   - SQL Server: `Server=localhost,1433;User Id=sa;Password=<yours>;TrustServerCertificate=True`
   - PostgreSQL: `Host=localhost;Port=5432;Username=<yours>;Password=<yours>;Database=occspec`
6. Stop when done: `docker compose --profile sqlserver down` (add `-v` to wipe data).

SQL files in `init/` run automatically the first time the PostgreSQL container starts — put your `CREATE TABLE` and seed scripts there.

Fallback: keep the same schema runnable on **SQLite** so the packaged prototype works with nothing installed. See `../notes/database-plan.md`.

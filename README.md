# EU5 Mod Planner

ASP.NET Core MVC planner for custom Europa Universalis V mod content, backed by PostgreSQL.

## Local development with Docker

1. Start PostgreSQL:

```powershell
docker compose up -d
```

2. Run the app:

```powershell
dotnet run
```

3. Open:

```text
http://localhost:5068
```

## Default local database settings

The app is configured to talk to the Docker database with this connection string:

```text
Host=localhost;Port=54329;Database=eu5_mod_planner_dev;Username=eu5planner;Password=eu5planner
```

ASP.NET configuration can override this through `ConnectionStrings__PlannerDatabase`.

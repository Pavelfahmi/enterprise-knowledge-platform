# Enterprise Knowledge Platform

AI-Powered Enterprise Knowledge and Support Platform — 60-day modern engineering capstone.

## Stack

- **.NET 10 (LTS)** — ASP.NET Core Minimal APIs
- Angular (frontend, coming next)
- PostgreSQL, Redis
- Docker / Docker Compose
- GitHub Actions → Azure Container Apps
- Semantic Kernel / Azure OpenAI (AI features)

## Why .NET 10 LTS (not 8 or 9)

- **.NET 8** is LTS but reaches end of support in **November 2026** — too short for a portfolio app you will keep deploying.
- **.NET 9** is **STS** (Standard Term Support), not LTS — shorter support window, not the right default for a production-oriented learning project.
- **.NET 10** is the current **LTS** release: longest support runway and the version this repo targets for all new API work.

See: https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core

## Repository layout

```
apps/api   — ASP.NET Core API
apps/web   — Angular app (planned)
infra/     — Azure / Bicep (planned)
tests/     — automated tests (planned)
```

## Local API (Day 1)

```
dotnet build
dotnet run --project apps/api
curl http://localhost:<port>/health
```

Expect a clean build (warnings as errors) and `Healthy` from `/health`.

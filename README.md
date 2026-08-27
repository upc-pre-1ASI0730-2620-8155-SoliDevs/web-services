# Soli-Devs — Web Services

RESTful API del modelo de negocio digital.
Curso **1ASI0730 – Aplicaciones Web** — UPC, Ciclo 2026-20.

## Tech stack

- [ASP.NET Core](https://dotnet.microsoft.com/apps/aspnet) (Web API) + **C#**
- [Entity Framework Core](https://learn.microsoft.com/en-us/ef/core/) (ORM)
- DBMS relacional: MySQL / PostgreSQL
- Documentación: **OpenAPI Specification** vía Swagger (default language: English)
- Pruebas unitarias y de integración incluidas en este repositorio

## Architecture

Bounded Contexts (Domain-Driven Design) gestionados de forma modular:

- Identity & Access Management
- Profiles & Preferences Management
- Subscriptions & Payment Management
- Bounded contexts core del dominio del negocio

## Getting started

```bash
git clone https://github.com/Soli-Devs/web-services.git
cd web-services
dotnet restore
dotnet ef database update
dotnet run
# Swagger UI available at /swagger
```

## Version control workflow

- **GitFlow**: `main` (releases) / `develop` (integración) / `feature/*` branches
- **Conventional Commits** + **Semantic Versioning**

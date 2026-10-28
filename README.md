# Mohamed Wael

**.NET Developer — C# · ASP.NET Core · SQL Server**

I build business web applications on .NET — multi-tenant SaaS, role & permission
systems, and back-office workflows. Currently building a multi-tenant practice
management platform for law offices.

Open to .NET roles and freelance projects.

---

## Tech I use

| Area | Tools |
|---|---|
| Language & frameworks | C#, ASP.NET Core (MVC, Web API), Razor |
| Data | SQL Server, Entity Framework Core (Code-First, Migrations), LINQ |
| Architecture | Clean Architecture, CQRS with MediatR, FluentValidation, Repository / Unit of Work, Specification pattern |
| Security | ASP.NET Core Identity, JWT, permission-based authorization, Google external login |
| Integrations | Redis caching, Stripe payments, MailKit, ClosedXML (Excel export), Serilog |
| Testing | xUnit, EF Core InMemory |

---

## Featured work

### Legal Practice Management SaaS — *private, commercial*
A multi-tenant web platform for law offices (Arabic, RTL), in production use by a law office.

- **Database-per-tenant** isolation — a master database holds the tenant registry; the tenant is resolved per request from the subdomain
- Modules: clients, cases, hearings with a calendar, case documents, employees, users & roles
- Fine-grained `{module}.{action}` permission system on top of ASP.NET Core Identity
- Per-tenant isolated file storage, printable views and Excel export
- Pending migrations applied to every tenant database on startup, with a backup first

`.NET 10` · `ASP.NET Core MVC` · `EF Core` · `SQL Server` · `MediatR` · `FluentValidation` · `Serilog` · `xUnit`

### Qassetly — Installment & Contract Management — *private*
A web system for managing customer contracts and installment schedules (Arabic, RTL).

- Modules: customers, categories & products, contracts, installments, payments and payment methods
- Custom permission-based authorization (`IAuthorizationPolicyProvider` + `IAuthorizationHandler`) with a global fallback policy
- Monthly installment calendar (FullCalendar, RTL), DataTables lists
- Core / Infrastructure / Web layering with a generic repository and Unit of Work

`.NET 9` · `ASP.NET Core MVC` · `EF Core` · `SQL Server` · `ASP.NET Core Identity`

> The source code of both projects is private. I'm happy to walk through the architecture in an interview.

### [StoreAPI](https://github.com/mohamed-wael15/StoreAPI) — E-commerce REST API *(training project)*
Layered Web API (Data / Repository / Service / Web) with JWT authentication,
Redis response caching, Stripe payment intents, the Specification pattern
and global exception-handling middleware.

`ASP.NET Core 8 Web API` · `EF Core` · `SQL Server` · `Redis` · `Stripe` · `Swagger`

---

## Training projects
- [MVC-CompanyAPP](https://github.com/mohamed-wael15/MVC-CompanyAPP) — employee & department management with Identity roles, Unit of Work and AutoMapper
- [E-CommerceWebApp](https://github.com/mohamed-wael15/E-CommerceWebApp) — online store (MVC) with Google login, a paginated catalog with search, and a cart *(work in progress)*

---

## Contact
- Email: waael3741@gmail.com
- LinkedIn: [mohamed-waael](https://www.linkedin.com/in/mohamed-waael-44a932303)

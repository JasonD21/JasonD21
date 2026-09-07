# Hi, I'm Jason 👋

Full-stack developer based in Cape Town, South Africa. I build web applications end-to-end — React and Angular frontends, C#/.NET backends, and the deployment infrastructure between them.

I'm the technical co-founder of **Meridian Worx**, where I design, build, and run [ClearOps](https://clearops.pages.dev) — a platform connecting trained workers with SMEs that need accurate, secure back-office data processing.

## 🔨 What I'm building

**[ClearOps](https://clearops.pages.dev)** — a production SaaS platform where I own the entire technical stack:

- **Frontend:** React 19 + TypeScript (strict), Vite, TanStack Query, React Hook Form + Zod, shadcn/ui on Tailwind CSS v4 — deployed on Cloudflare Pages
- **Backend:** ASP.NET Core (`net9.0`) Web API in a three-project Clean Architecture, EF Core + PostgreSQL, ASP.NET Identity with short-lived JWTs and rotating HttpOnly refresh cookies, SignalR for live updates — deployed on Railway via Docker
- **Also in the mix:** Cloudflare R2 object storage, a walled in-browser document viewer with per-render watermark auditing, Web Push, PayFast payments, Serilog + Sentry
- **Quality:** **722 automated tests across four layers** — xUnit + SQLite in-memory, Vitest + Testing Library, Playwright against a stubbed API, and a full-stack Playwright layer running against a real API and real Postgres to catch frontend/backend contract drift. CI/CD on GitHub Actions gates every PR.

> Source is private (commercial product) — I'm happy to walk through the architecture and code in an interview.
> 📖 [Full case study — architecture and engineering decisions →](https://github.com/JasonD21/clearops-case-study)

## 🔭 On the horizon

What I'm building into ClearOps next, and the engineering problem behind each:

- **Verifiable proof of review.** Every delivered batch carries an assurance record — who reviewed it, what was checked, first-pass accuracy, turnaround against SLA — snapshotted at delivery and never recomputed, plus a public verification page so the record survives being forwarded to an accountant. The interesting constraint is immutability: a document whose stated accuracy could change after delivery isn't evidence.
- **A client data layer.** Captured invoice data currently lives as untyped text per submission, which is fine for one batch and unusable across twelve months. Building a typed, indexed projection alongside the immutable source — rebuildable from it, never authoritative over it.
- **A findings engine with two renderings.** One rule set that produces both a reviewer-facing check and a client-facing finding, because maintaining two rule sets guarantees they drift.
- **Auto-graded skills training.** Practice tasks graded against stored answer keys with per-field feedback, replacing human grading that competes directly with production review for the same reviewers' time.
- **A second document pipeline** (bank statements), which needs the capture engine to handle many rows per document rather than one.

## 🚀 Recently shipped

**[successwithafrikaans.com](https://successwithafrikaans.com)** — marketing site + CMS for a tutoring business:

- Astro with React islands, TypeScript, Tailwind CSS v4, Sanity CMS, Cloudflare Pages Functions, Resend
- Strong Lighthouse scores and passing Google Rich Results validation
- 📖 [Full case study with screenshots and architecture →](https://github.com/JasonD21/successwithafrikaans-case-study)

## 🧰 Tech I work with

**Frontend:** React · Angular · TypeScript · Tailwind CSS · shadcn/ui · Astro
**Backend:** C# · ASP.NET Core · EF Core · SignalR · Node.js/Express
**Data & infra:** PostgreSQL · MongoDB · Firebase · Cloudflare (Pages, Functions, R2) · Docker · GitHub Actions
**Testing:** xUnit · NSubstitute · Shouldly · Vitest · Testing Library · Playwright · Karma/Jasmine

## 📫 Get in touch

- 💼 [LinkedIn](https://www.linkedin.com/in/jason-davids-09aa201b0/)
- ✉️ jasondavids54@gmail.com

*Open to remote freelance and contract opportunities.*

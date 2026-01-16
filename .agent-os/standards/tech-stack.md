# Tech Stack

> Version: 1.0.0
> Last Updated: 2025-08-31

## Context

This file is part of the Agent OS standards system. These global tech stack defaults are referenced by all product codebases when initializing new projects. Individual projects may override these choices in their `.agent-os/product/tech-stack.md` file.

## Core Technologies

### Application Framework
- **Framework:** FastAPI, pdm with uv
- **Version:** 0.116.1+
- **Language:** Python 3.10+

### Database
- **Primary:** PostgreSQL
- **Version:** 17+
- **ORM:** SQLModel and/or Drizzle

## Frontend Stack

### JavaScript Framework
- **Framework:** Next.js
- **Version:** Latest stable
- **Build Tool:** Turbopack

### Import Strategy
- **Strategy:** ES Modules
- **Package Manager:** pnpm
- **Node Version:** 22 LTS

### CSS Framework
- **Framework:** TailwindCSS & Radix UI
- **Version:** TailwindCSS 4.0+ & Radix UI 3.0.0+
- **PostCSS:** Yes

### UI Components
- **Library:** ShadCN
- **Version:** Latest
- **Installation:** CLI: pnpm dlx shadcn-ui@latest init

## Assets & Media

### Fonts
- **Provider:** FontShare
- **Loading Strategy:** Self-hosted for performance

### Icons
- **Libraries:** HeroIcons, Phosphoricons or Lucide
- **Implementation:** React components

## Infrastructure

### Application Hosting
- **Platform:** Vercel, Cloudflare, AWS, GCP, Railway, or Fly.io
- **Service:** Vercel: Vercel, Cloudflare: Cloudflare Pages or Cloudflare Workers, AWS: Elastic Beanstalk or Lambda, GCP: Cloud Run or App Engine, Railway: Deployments, Fly.io: Fly App
- **Region:** Primary region based on user base

### Database Hosting
- **Provider:** Supabase, Neon or Turso
- **Service:** Managed PostgreSQL
- **Backups:** Daily automated

### Asset Storage
- **Provider:** Amazon S3
- **CDN:** CloudFront
- **Access:** Private with signed URLs

## Deployment

### CI/CD Pipeline
- **Platform:** GitHub Actions
- **Trigger:** Push to main/staging branches
- **Tests:** Run before deployment

### Environments
- **Production:** main branch
- **Staging:** staging branch
- **Review Apps:** PR-based (optional)

---

*Customize this file with your organization's preferred tech stack. These defaults are used when initializing new projects with Agent OS.*

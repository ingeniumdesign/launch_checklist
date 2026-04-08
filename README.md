# Launch Checklist

**Your Go-Live Companion — Nothing Gets Forgotten.**

A structured, automated checklist system for website launches. Over 200 pre-built tasks, 9 automated verification checks, team collaboration, and real-time progress tracking — so nothing slips through the cracks.

🌐 **[launch-checklist.com](https://launch-checklist.com)**

---

## Try It Now — Free, No Registration

Start using Launch Checklist **instantly** — no signup, no credit card, no commitment:

1. Choose a template (Default, TYPO3, WordPress)
2. Start checking off tasks
3. Export your progress as PDF
4. Register later to save your data permanently (seamless, no data loss)

👉 **[Start your free checklist now](https://launch-checklist.com/checklist)**

---

## Screenshot

<!-- Replace with actual screenshot -->
> Visit **[launch-checklist.com](https://launch-checklist.com)** to see it live.

---

## Key Features

### Structured Checklists

Over **213 pre-built tasks** organized in **20 categories**, covering everything from DNS setup to post-launch monitoring. Each task includes:

- **Why it matters** — contextual explanation of the task's importance
- **How to fix it** — actionable guidance on how to complete it
- **Documentation links** — direct links to official references (51 tasks)
- **Priority level** — Strong, Normal, or Low
- **Drag & Drop** — Reorder tasks within categories to match your workflow

**Categories include:**
Project Organisation, Domain & DNS, Hosting & Infrastructure, SSL & HTTPS, Security, SEO, Robots & Indexing, Redirects & URL Structure, Content, Media & Assets, Design & UX, Performance, Forms & Leads, Tracking & Analytics, Privacy & Legal, Email & Notifications, CMS Backend, Backups & Recovery, Monitoring & Post-Launch, Finalisation & Documentation.

### 9 Automated Checks (Verify System)

Don't just check off tasks manually — let the system **verify them automatically**:

| Check | What It Verifies |
|-------|-----------------|
| **SSL Certificate** | HTTPS reachable, certificate expiry, self-signed detection |
| **robots.txt** | Valid directives, site self-blocking detection, meta noindex/nofollow |
| **sitemap.xml** | Resolves from robots.txt, fallback paths, validates XML |
| **HTTPS Redirect** | HTTP → HTTPS (301/302/307/308), SEO recommendations |
| **Security Headers** | X-Frame-Options, X-Content-Type-Options, HSTS with value validation |
| **Canonical Tag** | HTML tag + HTTP header, multiple tags, www mismatch detection |
| **Meta Tags** | Title/description length, viewport, lang, charset |
| **Open Graph** | og:title, og:image, og:description, image reachability |
| **Favicon** | HTML link tags, /favicon.ico, Apple Touch Icon, manifest |

Works with **password-protected staging environments** (Basic Auth support). Tasks are automatically checked off when verification passes. When a check **fails**, the system provides **specific fix guidance** — explaining why it matters and exactly how to resolve the issue.

### Project Templates

Start with pre-configured templates for different website types:

- **Default** — Universal checklist for any website
- **TYPO3** — Extended with CMS-specific tasks (cache, extensions, TypoScript)
- **WordPress** — Extended with plugin, theme, and security tasks

Save your own project configurations as **reusable templates** for future launches.

### Team Collaboration

Work together on launches with your team:

- **Team roles** — Owner, Admin, Member with granular permissions
- **Task assignment** — Assign tasks to specific team members
- **Comments** — Add notes and discussions per task
- **Email invitations** — Invite team members with one click
- **Multiple teams** — Manage different teams for different clients

### Share Projects — No Login Required

Share any project with stakeholders via a **unique read-only link**:

- **No account needed** — recipients just open the link
- **Optional password** protection (AES-256-GCM encrypted)
- **Configurable expiry** — 7 days, 30 days, or unlimited
- **Live data** — viewers always see current progress (auto-refresh)
- **PDF export** available directly from the shared view

Perfect for sharing launch progress with clients who don't need an account.

### Project Lifecycle

Track your project through its natural lifecycle:

- **Active** → **Completed** (with confetti celebration!) → **Archived**
- Reopen completed projects or unarchive archived ones
- Only team Owners and Admins can manage project status

### Export & Reporting

Generate professional reports in multiple formats:

- **PDF** — For stakeholders and project documentation
- **Markdown** — For wikis and documentation systems
- **JSON** — For integrations and automation
- **Redmine** — Compatible with Redmine project management

### Passwordless Login

- **Magic Link** — Receive a login link via email, no password needed
- **Password Reset** — "Forgot password?" flow with secure email tokens
- **Rate Limited** — All auth endpoints protected against brute-force
- **Anti-Enumeration** — Auth flows never reveal if an email exists

### Admin Panel

Full control over the system:

- **Task Pool** — Manage all 213 tasks (edit, activate/deactivate, documentation links)
- **User Management** — View users, change roles, team overview
- **System Settings** — SMTP, app name, invitation expiry — all configurable via UI
- **Dashboard** — KPI overview with charts (projects, teams, users, task completion)
- **SMTP Test** — Verify email configuration directly from the admin panel

### Dark Mode & Multilingual

- **Dark and Light mode** with automatic system detection
- Full support for **English** and **German** — including all 213 task definitions
- **Localized URLs** — `/projects` (EN) → `/de/projekte` (DE)
- Adding more languages is as simple as adding one translation file

---

## Privacy First

Launch Checklist takes a **privacy-first approach**:

- **No tracking** — No Google Analytics, no Facebook Pixel, no third-party scripts
- **No consent banner needed** — Only functional cookies (session, team context)
- **Self-hosted** — Your data stays on your server
- **GDPR-compliant** — Full privacy policy included, IP logging with SHA-256 hashing
- **Fonts self-hosted** — No Google Fonts CDN, no external requests

---

## Self-Hosting (Docker)

Deploy on your own server with **zero configuration**:

```bash
docker compose up -d --build
```

That's it. The system automatically:
1. Creates the database
2. Runs all migrations
3. Seeds initial data (213 tasks, categories, templates, admin user)
4. Starts the application

**Update workflow** — just as simple:

```bash
git pull && docker compose up -d --build
```

New migrations and seed data are applied automatically on every start.

**Requirements:** Docker + Docker Compose. Runs on any Linux server (tested on Ubuntu 24.04).

---

## Built With

| Technology | Purpose |
|-----------|---------|
| [Next.js](https://nextjs.org) | React framework (App Router, Server Components) |
| [TypeScript](https://www.typescriptlang.org) | Type-safe development |
| [PostgreSQL](https://www.postgresql.org) | Reliable database |
| [Prisma](https://www.prisma.io) | Type-safe ORM with migrations |
| [Tailwind CSS](https://tailwindcss.com) | Utility-first styling |
| [shadcn/ui](https://ui.shadcn.com) | UI component library |
| [Auth.js](https://authjs.dev) | Authentication (credentials + magic link) |
| [next-intl](https://next-intl.dev) | Internationalization with localized URLs |
| [Nodemailer](https://nodemailer.com) | Transactional email (invitations, magic links) |
| [Docker](https://www.docker.com) | Zero-config containerized deployment |

---

## Who Is It For?

- **Web agencies** managing multiple client launches
- **Freelancers** who want a professional launch process
- **Website owners** launching their first site
- **Development teams** deploying software and web applications
- **DevOps engineers** managing infrastructure go-lives

---

## About

Launch Checklist is developed by **[INGENIUMDESIGN](https://www.ingeniumdesign.de)** — a web agency specializing in professional web development and digital solutions.

---

## Links

- 🌐 **Website**: [launch-checklist.com](https://launch-checklist.com)
- 🚀 **Free Checklist**: [launch-checklist.com/checklist](https://launch-checklist.com/checklist)

---

*Launch Checklist — Because every successful launch starts with a checklist.* ✅

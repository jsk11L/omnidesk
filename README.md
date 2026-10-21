# OmniDesk

A personal workspace for calendars, notes, tasks, collections and finances.

## Overview

OmniDesk brings everyday organization into an Angular application backed by a NestJS API and PostgreSQL. The repository also includes an Android project using Capacitor.

## Features

- Calendar views with event reminders.
- Custom collections with fields, tags and cover images.
- Rich-text notes with autosave and search.
- Kanban boards with priorities and due dates.
- Finance boards, transactions, budgets and charts.
- In-app, browser push and email notifications.
- Preset and custom themes, plus a command palette.

## Tech stack

| Layer | Technologies |
| --- | --- |
| Frontend | Angular 18, TypeScript, Tailwind CSS, FullCalendar, TipTap, Chart.js |
| Backend | NestJS 10, Prisma, Passport JWT, Nodemailer, Web Push |
| Database | PostgreSQL |
| Mobile | Capacitor, Android |
| Infrastructure | pnpm workspace, Docker Compose, nginx |

## Getting started

Follow the [installation guide](docs/operations/install.md) for environment setup and the Docker workflow. It covers database credentials, JWT secrets and application URLs.

For local development, the root package declares Node.js 20+ and pnpm 9+. After configuring dependencies and the database, use `pnpm backend:dev` and `pnpm frontend:dev` in separate terminals.

Register an account, verify the email address and sign in to access the workspace. Notification delivery depends on the configured mail and push services.

## Documentation

- [Cloud deployment](docs/operations/deploy-cloudflare-render-neon.md)
- [HTTPS setup](docs/operations/https-setup.md)
- [Backup and restore](docs/operations/backup.md)
- [Database migrations](docs/operations/migrations.md)
- [Upgrades](docs/operations/upgrade.md) and [rollback](docs/operations/rollback.md)

## Project structure

`frontend/` contains the web application; `backend/` contains the API and Prisma schema; `shared/` holds shared types; `android/` contains the mobile project; `infra/` and `scripts/` support deployment and operations.

## Languages

Includes Spanish project materials alongside English documentation. This README is written in English.

## License

[MIT](LICENSE).

---

A project in [Javier Sepúlveda's portfolio](https://github.com/jsk11L).

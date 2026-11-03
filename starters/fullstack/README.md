# Fullstack Starter

Full app with frontend + backend + database (Next.js + Prisma + SQLite for zero-config dev).

## What is this?
A single Next.js app that serves both UI and API, with Prisma as ORM and SQLite for the database (no server to install).

## Prerequisites
- Node.js v18+  ->  `node -v`
- pnpm (or npm)  ->  `pnpm -v`

## Create your own copy
```bash
pnpm create next-app@latest my-app --ts --app --tailwind --eslint --src-dir --import-alias "@/*"
cd my-app
pnpm add prisma @prisma/client
pnpm prisma init --datasource-provider sqlite
```

Then edit `prisma/schema.prisma`, add a model, run:
```bash
pnpm prisma migrate dev --name init
pnpm prisma generate
pnpm dev
```

## Coming soon in this folder
A ready-to-run example app with:
- User model in Prisma
- REST API routes in `src/app/api/`
- A form that creates a record
- A list page that reads from the DB

## Project structure (once populated)
```
fullstack/
  prisma/
    schema.prisma
    dev.db
  src/
    app/
      api/
      page.tsx
    lib/
      db.ts
  package.json
```

## Next steps
- With AI: use [skills/build-fullstack-app.md](../../skills/build-fullstack-app.md)
- Without AI: https://www.prisma.io/docs/getting-started/quickstart


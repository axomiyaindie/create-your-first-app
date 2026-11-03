# Skill: Build a Fullstack App

**Goal:** Take a user from zero to a running fullstack app (Next.js + Prisma + SQLite) with a database, API, and UI - no prior coding knowledge.

## Prerequisites check
- `node -v` -> v18+
- `pnpm -v` (or `npm -v`)
- `git --version`

## Steps

1. **Scaffold**
   ```bash
   pnpm create next-app@latest my-app --ts --app --tailwind --eslint --src-dir --import-alias "@/*"
   cd my-app
   ```

2. **Add Prisma + SQLite**
   ```bash
   pnpm add prisma @prisma/client
   pnpm prisma init --datasource-provider sqlite
   ```

3. **Define a model** in `prisma/schema.prisma`:
   ```prisma
   model Post {
     id        Int      @id @default(autoincrement())
     title     String
     content   String
     createdAt DateTime @default(now())
   }
   ```

4. **Migrate + generate**
   ```bash
   pnpm prisma migrate dev --name init
   pnpm prisma generate
   ```

5. **Create the DB client** in `src/lib/db.ts`:
   ```ts
   import { PrismaClient } from "@prisma/client";
   const globalForPrisma = globalThis as unknown as { prisma?: PrismaClient };
   export const db = globalForPrisma.prisma ?? new PrismaClient();
   if (process.env.NODE_ENV !== "production") globalForPrisma.prisma = db;
   ```

6. **Add API routes**
   - `src/app/api/posts/route.ts` - GET (list) + POST (create)
   - `src/app/api/posts/[id]/route.ts` - GET one + DELETE

7. **Add UI**
   - `src/app/page.tsx` - form (create post) + list (read posts)
   - Use `fetch("/api/posts")` from a client component

8. **Ask the user what the app does** (one sentence). Rename `Post` and fields to match their domain.

9. **Run**
   ```bash
   pnpm dev
   ```
   Open http://localhost:3000

10. **Commit**
    ```bash
    git init && git add . && git commit -m "feat: initial fullstack app"
    ```

## Rules for the agent
- SQLite for local dev. Never commit `prisma/dev.db` (`.gitignore` handles it).
- All DB access goes through `src/lib/db.ts`.
- Validate input with Zod on the server side.
- Never expose secret keys to the client.
- Explain each command in one short sentence before running it.

## Done when
- `pnpm dev` runs without errors.
- Home page loads at localhost:3000.
- Submitting the form creates a record visible in the list.
- `pnpm prisma studio` shows the row in the DB.


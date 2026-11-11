# Skill: Build a Next.js App

**Goal:** Take a user from zero to a running Next.js app without prior coding knowledge.

## Prerequisites check
- node -v  (v18+)
- pnpm -v  (or npm -v)
- git --version

## Steps
1. Scaffold:
   pnpm create next-app@latest my-app --ts --app --tailwind --eslint --src-dir --import-alias "@/*"
   cd my-app

2. Install base deps:
   pnpm add lucide-react clsx

3. Ask the user what the app does (one sentence). Build:
   - 1 home page + 1 functional page
   - Tailwind styling
   - Small components in src/components/

4. Run:
   pnpm dev
   Open http://localhost:3000

5. Commit:
   git init && git add . && git commit -m "feat: initial nextjs app"

## Rules
- Use mock data first, never invent APIs.
- Prefer server components unless interactivity is required.
- Show the file tree after scaffolding.
- Explain each command in one short sentence before running it.

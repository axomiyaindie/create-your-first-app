# Skill: Build an Astro Site

**Goal:** Take a user from zero to a running Astro site (blog / docs / landing page) without prior coding knowledge.

## Prerequisites check
- `node -v` -> v18+
- `pnpm -v` (or `npm -v`)
- `git --version`

If missing, guide the user to https://nodejs.org and https://pnpm.io.

## Steps

1. **Scaffold**
   ```bash
   pnpm create astro@latest my-site -- --template minimal --typescript strict --install --git
   cd my-site
   ```

2. **Install extras**
   ```bash
   pnpm astro add tailwind
   pnpm add @astrojs/mdx
   pnpm astro add mdx
   ```

3. **Ask the user what the site is about** (one sentence). Then:
   - Create `src/layouts/BaseLayout.astro` (header, footer, Tailwind)
   - Create `src/pages/index.astro` (hero + 3 feature cards)
   - Create `src/content/blog/welcome.md` as a sample post
   - Create `src/pages/blog/[...slug].astro` to render posts
   - Add a dark-mode toggle (Tailwind + localStorage)

4. **Run locally**
   ```bash
   pnpm dev
   ```
   Open http://localhost:4321

5. **Commit**
   ```bash
   git add . && git commit -m "feat: initial astro site"
   ```

## Rules for the agent
- Content-first: default to Markdown for anything text-heavy.
- No client-side JS unless the feature needs it (Astro islands only).
- Every page must use `BaseLayout.astro`.
- Explain each command in one short sentence before running it.

## Done when
- `pnpm dev` runs without errors.
- Home page renders at localhost:4321.
- `/blog/welcome` shows the sample post.
- Dark-mode toggle works.


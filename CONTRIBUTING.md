# Contributing

Thanks for wanting to improve **create-your-first-app**! This repo is a collection of
starter templates and AI-agent skills for building apps with zero prior knowledge.

## Ways to contribute

1. **Add a new skill** -> drop a markdown file in `skills/`
2. **Add a new starter** -> create `starters/<name>/` with a working template + README
3. **Improve docs** -> edit anything under `docs/`
4. **Report bugs / suggest ideas** -> open an issue

## Skill format

Each skill is one markdown file in `skills/` named `build-<stack>-app.md`.
It must include:

- **Goal** - one sentence
- **Prerequisites** - commands to verify tools are installed
- **Steps** - numbered, each with a copy-paste command
- **Rules** - constraints for the AI agent
- **Done when** - acceptance criteria

See `skills/build-nextjs-app.md` as the reference template.

## Starter format

Each folder in `starters/<name>/` must contain:

- A working, runnable minimal app
- `README.md` with: what it is, prerequisites, how to run, project structure, next steps
- No secrets, no `node_modules`, no build artifacts (`.gitignore` handles most)

## Commit style

Use conventional commits:

- `feat: add astro starter`
- `docs: expand flutter skill`
- `fix: correct tauri init command`
- `chore: update gitignore`

## Pull request checklist

- [ ] Files follow the format above
- [ ] `README.md` of the starter runs from a clean clone
- [ ] No secrets or large binaries
- [ ] `git status` is clean after commit

## Code of conduct

Be kind. Assume good intent. No harassment, no spam, no crypto shilling.

# Repository Structure

A navigation guide to help you find the right resources, explore projects, and understand how everything is organized inside **Create Your First App**.

You don't need to explore the entire repository. Start with the section that matches what you want to do.

## Where should I go?

| I want to... | Go to |
|---|---|
| Build my first application | [`docs/getting-started/`](docs/getting-started/README.md) |
| Explore ready-to-use starter projects | [`starters/`](starters/README.md) |
| Learn how to build with AI coding agents | [`skills/`](skills/README.md) |
| Set up or configure an AI coding agent | [`agents/`](agents/README.md) |
| Understand programming and development fundamentals | [`docs/fundamentals/`](docs/fundamentals/README.md) |
| Learn about web development | [`skills/web-development/`](skills/web-development/README.md) |
| Build mobile applications | [`skills/mobile-development/`](skills/mobile-development/README.md) |
| Build desktop applications | [`skills/desktop-development/`](skills/desktop-development/README.md) |
| Build backend or full-stack applications | [`skills/backend-development/`](skills/backend-development/README.md) |
| Deploy an application | [`docs/deployment/`](docs/deployment/README.md) |
| Troubleshoot a development problem | [`docs/troubleshooting/`](docs/troubleshooting/README.md) |
| Contribute to this project | [`CONTRIBUTING.md`](CONTRIBUTING.md) |

---

## Repository map

```text
create-your-first-app/
│
├── README.md
├── STRUCTURE.md
├── LICENSE
├── CONTRIBUTING.md
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
│
├── agents/                         # AI coding agent configurations
│   ├── claude-code/
│   ├── codex/
│   ├── cursor/
│   ├── gemini-cli/
│   └── github-copilot/
│
├── assets/                         # Project branding and visual assets
│   └── branding/
│
├── docs/                           # Learning resources and documentation
│   ├── getting-started/
│   ├── fundamentals/
│   ├── ai-agents/
│   ├── deployment/
│   ├── troubleshooting/
│   └── faq/
│
├── skills/                         # Reusable AI development instructions
│   ├── web-development/
│   ├── mobile-development/
│   ├── desktop-development/
│   ├── backend-development/
│   └── fullstack-development/
│
├── starters/                       # Application starter projects
│   ├── web/
│   │   ├── nextjs/
│   │   └── astro/
│   │
│   ├── mobile/
│   │   ├── android/
│   │   ├── flutter/
│   │   └── ios/
│   │
│   ├── desktop/
│   │   ├── windows/
│   │   ├── macos/
│   │   ├── linux/
│   │   └── tauri/
│   │
│   ├── backend/
│   │   ├── node-express/
│   │   └── python-fastapi/
│   │
│   └── fullstack/
│       └── nextjs-prisma/
│
├── templates/                      # Reusable project and skill templates
│   ├── skill-template.md
│   └── starter-template/
│
├── scripts/                        # Repository maintenance scripts
│   └── validate-repository/
│
└── .github/                        # GitHub workflows and contribution templates
    ├── ISSUE_TEMPLATE/
    ├── workflows/
    └── PULL_REQUEST_TEMPLATE.md
```

*Note: A listed directory may contain documentation or planned resources rather than a complete, runnable project. Check its README before using it.*

---

## 1. Documentation — `docs/`

Start here if you want to understand application development, learn the fundamentals, or follow a guided learning path.

| Directory | Purpose |
|---|---|
| `getting-started/` | Your first steps with this repository |
| `fundamentals/` | Core development concepts |
| `ai-agents/` | Understanding and working with AI coding agents |
| `deployment/` | Publishing and deploying applications |
| `troubleshooting/` | Common problems and solutions |
| `faq/` | Frequently asked questions |

**Start here:** [`docs/README.md`](docs/README.md)

## 2. Development Skills — `skills/`

Skills are reusable instruction files that help AI coding agents plan, build, and improve applications.

| Category | Purpose |
|---|---|
| `web-development/` | Websites and web applications |
| `mobile-development/` | Android, iOS, and Flutter applications |
| `desktop-development/` | Cross-platform and native desktop applications |
| `backend-development/` | APIs, servers, and backend systems |
| `fullstack-development/` | Complete frontend and backend applications |

**Start here:** [`skills/README.md`](skills/README.md)

## 3. Starter Projects — `starters/`

Explore starter projects organized by application platform and technology.

| Category | Technologies |
|---|---|
| `web/` | Next.js, Astro |
| `mobile/` | Android, Flutter, iOS |
| `desktop/` | Windows, macOS, Linux, Tauri |
| `backend/` | Node.js and Express, Python and FastAPI |
| `fullstack/` | Next.js and Prisma |

Each starter should have its own README describing its purpose, requirements, setup instructions, and testing status.

**Start here:** [`starters/README.md`](starters/README.md)

## 4. AI Agent Configurations — `agents/`

Find configuration examples and guidance for different AI coding environments.

- Claude Code
- OpenAI Codex
- Cursor
- Gemini CLI
- GitHub Copilot

**Start here:** [`agents/README.md`](agents/README.md)

## 5. Templates — `templates/`

Reusable starting points for creating new skills and application starter projects.

- `skill-template.md` — Structure for writing a reusable development skill.
- `starter-template/` — Structure for contributing a new starter project.

**Start here:** [`templates/README.md`](templates/README.md)

## 6. Project Assets — `assets/`

Branding resources, logos, icons, and other visual assets used by the repository.

**Start here:** [`assets/branding/README.md`](assets/branding/README.md)

## 7. Repository Maintenance

| File or directory | Purpose |
|---|---|
| `.github/workflows/` | Automated repository checks |
| `.github/ISSUE_TEMPLATE/` | Issue submission templates |
| `.github/PULL_REQUEST_TEMPLATE.md` | Pull request guidance |
| `scripts/` | Validation and maintenance scripts |
| `CONTRIBUTING.md` | Contribution guidelines |
| `CHANGELOG.md` | Project changes |
| `SECURITY.md` | Security reporting |
| `CODE_OF_CONDUCT.md` | Community standards |

---

## Understanding resource availability

We want visitors to know exactly what they can use today.

- **Guide available:** Documentation or instructions are provided.
- **Starter available:** Actual application source code is included.
- **Tested:** Setup and documented acceptance checks have been successfully verified.

A guide is not automatically a runnable application. Always check the individual resource's README for its current status.

---

## Not sure where to start?

- **Complete beginner:** Start with [`Getting Started`](docs/getting-started/README.md).
- **Want to build something immediately:** Explore [`Starter Projects`](starters/README.md).
- **Already know development:** Explore [`Development Skills`](skills/README.md).
- **Want to use an AI coding agent:** Explore [`Agent Configurations`](agents/README.md).

**Back to the [main README](README.md).**
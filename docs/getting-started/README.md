# Getting Started

New to programming? This guide helps you prepare your computer, choose a technology, and use an AI coding agent to build your first application.

You do not need to understand every line of code before you begin. You should, however, review what your AI agent creates and ask it to explain unfamiliar decisions.

## 1. Choose what you want to build

| Your goal | Starter documentation | Development guide |
|---|---|---|
| Website or web application | [Next.js](../../starters/web/nextjs/) | [Next.js guide](../../skills/web-development/build-nextjs-app.md) |
| Blog or content website | [Astro](../../starters/web/astro/) | [Astro guide](../../skills/web-development/build-astro-site.md) |
| Cross-platform mobile app | [Flutter](../../starters/mobile/flutter/) | [Flutter guide](../../skills/mobile-development/build-flutter-app.md) |
| Native Android app | [Android](../../starters/mobile/android/) | [Android guide](../../skills/mobile-development/build-android-app.md) |
| Desktop application | [Tauri](../../starters/desktop/tauri/) | [Tauri guide](../../skills/desktop-development/build-tauri-desktop.md) |
| Full-stack application | [Next.js and Prisma](../../starters/fullstack/nextjs-prisma/) | [Full-stack guide](../../skills/fullstack-development/build-fullstack-app.md) |

Check each starter's README to see whether it contains a runnable project or documentation only.

## 2. Install the essentials

You will generally need Git, Node.js, a code editor, and an AI coding agent. Individual technologies may require additional tools.

### Windows

Open PowerShell:

```powershell
winget install Git.Git
winget install OpenJS.NodeJS.LTS
winget install Microsoft.VisualStudioCode
npm install -g pnpm
```

Restart your terminal after installation.

### macOS

Open Terminal:

```bash
brew install git node pnpm
brew install --cask visual-studio-code
```

### Linux

On Debian or Ubuntu:

```bash
sudo apt update
sudo apt install -y git nodejs npm
sudo npm install -g pnpm
```

Check the official Node.js installation instructions if your distribution provides an outdated version.

### Verify the installations

```bash
git --version
node --version
npm --version
pnpm --version
```

Use the current supported Node.js LTS release and check the selected technology's requirements.

## 3. Choose an AI coding agent

Some options include:

- [Claude Code](https://claude.com/product/claude-code)
- [OpenAI Codex](https://openai.com/codex/)
- [Cursor](https://cursor.com/)
- [GitHub Copilot](https://github.com/features/copilot)
- [Gemini CLI](https://github.com/google-gemini/gemini-cli)

Choose an agent that can access your project files and run terminal commands, if you want it to scaffold and test the application directly.

## 4. Give the agent a development guide

For example, if you want to build a Next.js application:

1. Open [the Next.js development guide](../../skills/web-development/build-nextjs-app.md).
2. Copy its instructions into your AI coding agent, or point the agent to the file if it can access the repository.
3. Describe the application you want to create.
4. Ask the agent to explain the important steps, implement the application, and verify that it works.

A useful first prompt:

```text
Follow the Next.js development guide.

I am new to programming. Help me build a personal portfolio website.

Explain the important steps, create the project, run it locally,
and verify that the main features work.

Do not skip setup instructions or silently ignore errors.
```

## 5. Run your application

The development guide should explain how to create the project and install its dependencies.

For a typical Next.js project, the commands after scaffolding are:

```bash
pnpm install
pnpm dev
```

Open the local address shown in the terminal, usually `http://localhost:3000`.

These commands assume the AI agent has already created a Next.js project in the current directory. They will not work inside this repository's documentation-only starter directory.

## 6. Learn as you build

- Read the [FAQ](../faq/README.md) for common problems.
- Browse the [development skills](../../skills/README.md).
- Explore the [application starters](../../starters/README.md).
- Learn about [AI coding agents](../../agents/README.md).
- Read the [contribution guidelines](../../CONTRIBUTING.md).

## 7. Save your work

When your project is working, you can save it with Git:

```bash
git init
git add .
git commit -m "feat: create my first application"
```

You can later publish your project to a Git hosting service.

## Need help?

If you encounter a problem with this repository, check the FAQ or [open an issue](https://github.com/axomiyaindie/create-your-first-app/issues).

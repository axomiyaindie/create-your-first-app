# Getting Started

New to coding? Start here. This page takes you from **nothing installed** to a **running app** in about 20 minutes.

## 1. What do you want to build?

| I want to build... | Go to starter | Skill to use with AI |
|---|---|---|
| A website or web app | [starters/nextjs](../../starters/nextjs/) | [skills/build-nextjs-app.md](../../skills/build-nextjs-app.md) |
| A blog / content site | [starters/astro](../../starters/astro/) | [skills/build-astro-site.md](../../skills/build-astro-site.md) |
| A mobile app (iOS + Android) | [starters/flutter](../../starters/flutter/) | [skills/build-flutter-app.md](../../skills/build-flutter-app.md) |
| A native Android app | [starters/android](../../starters/android/) | [skills/build-android-app.md](../../skills/build-android-app.md) |
| A desktop app (Win/Mac/Linux) | [starters/tauri](../../starters/tauri/) | [skills/build-tauri-desktop.md](../../skills/build-tauri-desktop.md) |
| A full app with backend + database | [starters/fullstack](../../starters/fullstack/) | [skills/build-fullstack-app.md](../../skills/build-fullstack-app.md) |

## 2. Install the essentials (once)

You need **Node.js**, **Git**, and a code editor. Pick your OS:

### Windows
```powershell
winget install OpenJS.NodeJS.LTS
winget install Git.Git
npm install -g pnpm
winget install Microsoft.VisualStudioCode
```

### macOS
```bash
brew install node git pnpm
brew install --cask visual-studio-code
```

### Linux (Debian/Ubuntu)
```bash
sudo apt update
sudo apt install -y nodejs npm git
sudo npm install -g pnpm
```

### Verify everything works
```bash
node -v      # v18 or higher
npm -v
pnpm -v
git --version
```

## 3. Use an AI agent (optional but powerful)

You do **not** need to know how to code. Open one of these:

- **Claude** - https://claude.ai
- **Cursor** - https://cursor.com
- **GitHub Copilot** - inside VS Code

Then:

1. Open the skill file for your stack (e.g. `skills/build-nextjs-app.md`)
2. Copy the whole file into the AI chat
3. Say: *"Follow this skill. Build me a [your idea]."*
4. Let it work. Ask questions if anything fails.

## 4. Typical first session

```bash
cd starters/nextjs
cat README.md
pnpm install
pnpm dev
```

Open the URL shown (usually http://localhost:3000) - you have a running app.

## 5. What next?

- Read the [FAQ](../faq/) for common problems
- Browse [skills/](../../skills/) for step-by-step build instructions
- Commit your work: `git add . && git commit -m "feat: my first app"`

## Still stuck?

Open an issue: https://github.com/axomiyaindie/create-your-first-app/issues


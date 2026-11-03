# create-your-first-app

**Start building real apps - web, mobile, and desktop - even if you have never coded before.**

This repo gives you:

- 🚀 **Starter templates** for popular stacks (Next.js, Astro, Flutter, Android, Tauri, plus a backend folder)
- 🤖 **AI agent skills** - plain-markdown instruction packs you paste into Claude / Cursor / Copilot so the AI knows exactly how to build each kind of app
- 📚 **Beginner docs** - install guides and a big FAQ for the errors you will actually hit
- 🧩 **Placeholders** for platforms that are not built yet (iOS, macOS, Linux) - contribute yours

> **No prior coding knowledge required.** Pick a stack, copy the matching skill into your AI agent, and describe what you want to build.

---

## 🎯 What do you want to build?

| I want to build... | Starter | AI skill | Status |
|---|---|---|---|
| A website / web app | [starters/nextjs](starters/nextjs/) | [build-nextjs-app.md](skills/build-nextjs-app.md) | ✅ ready to use |
| A blog / content site | [starters/astro](starters/astro/) | [build-astro-site.md](skills/build-astro-site.md) | ✅ ready to use |
| A cross-platform mobile app | [starters/flutter](starters/flutter/) | [build-flutter-app.md](skills/build-flutter-app.md) | ✅ ready to use |
| A native Android app | [starters/android](starters/android/) | [build-android-app.md](skills/build-android-app.md) | ✅ ready to use |
| A Windows desktop app | [starters/tauri](starters/tauri/) | [build-tauri-desktop.md](skills/build-tauri-desktop.md) | ✅ ready to use |
| A full app with backend + DB | [starters/fullstack](starters/fullstack/) | [build-fullstack-app.md](skills/build-fullstack-app.md) | ✅ ready to use |
| A separate backend API | [starters/backend](starters/backend/) | use the fullstack skill | 🚧 placeholder |
| An iOS app | [starters/ios](starters/ios/) | (coming) | 🚧 placeholder |
| A macOS desktop app | [starters/macos](starters/macos/) | (coming) | 🚧 placeholder |
| A Linux desktop app | [starters/linux](starters/linux/) | (coming) | 🚧 placeholder |

---

## ⚡ Quick start (3 minutes)

### 1. Install the basics (once per computer)

**Windows (PowerShell):**
```powershell
winget install OpenJS.NodeJS.LTS
winget install Git.Git
winget install Microsoft.VisualStudioCode
npm install -g pnpm
```

**macOS:**
```bash
brew install node git pnpm
brew install --cask visual-studio-code
```

**Linux (Debian/Ubuntu):**
```bash
sudo apt install -y nodejs npm git
sudo npm install -g pnpm
```

### 2. Pick a starter
Browse the table above or open [`starters/`](starters/).

### 3. Build it with AI (optional but powerful)
1. Open **Claude**, **Cursor**, or **GitHub Copilot**
2. Paste the matching skill file (e.g. `skills/build-nextjs-app.md`) into the chat
3. Say: *"Follow this skill. Build me a [your idea]."*

That is it. The AI scaffolds the project, installs dependencies, and writes the code while following the rules in the skill.

---

## 📁 Repo structure

```
create-your-first-app/
├── README.md              ← you are here
├── CONTRIBUTING.md        ← how to add your own starter or skill
├── LICENSE                ← MIT
├── docs/
│   ├── getting-started/   ← zero-to-running guide for beginners
│   └── faq/               ← install errors, git problems, AI issues
├── skills/                ← AI agent instruction packs (one per stack)
│   ├── build-nextjs-app.md
│   ├── build-astro-site.md
│   ├── build-flutter-app.md
│   ├── build-android-app.md
│   ├── build-tauri-desktop.md
│   └── build-fullstack-app.md
└── starters/              ← starter templates
    ├── nextjs/            ✅ ready
    ├── astro/             ✅ ready
    ├── flutter/           ✅ ready
    ├── android/           ✅ ready
    ├── tauri/             ✅ ready (Windows verified)
    ├── fullstack/         ✅ ready
    ├── backend/           🚧 placeholder
    ├── ios/               🚧 placeholder
    ├── macos/             🚧 placeholder
    └── linux/             🚧 placeholder
```

---

## 🤖 What is an "AI agent skill"?

A skill is a plain markdown file that tells an AI agent *exactly* how to build a specific kind of app. It contains:

- **Goal** - what the agent will produce
- **Prerequisites** - tools the user must have installed
- **Steps** - numbered, command-first instructions
- **Rules** - constraints so the agent does not improvise
- **Done when** - acceptance criteria

You do not need to understand every line. Just paste it into your AI agent and follow along. The agent reads the rules, scaffolds the project, and explains each command.

Skills in this repo:
- [`build-nextjs-app.md`](skills/build-nextjs-app.md)
- [`build-astro-site.md`](skills/build-astro-site.md)
- [`build-flutter-app.md`](skills/build-flutter-app.md)
- [`build-android-app.md`](skills/build-android-app.md)
- [`build-tauri-desktop.md`](skills/build-tauri-desktop.md)
- [`build-fullstack-app.md`](skills/build-fullstack-app.md)

---

## 🧠 No prior coding knowledge? Start here

1. Read [`docs/getting-started/`](docs/getting-started/) - install guides for Windows, macOS, Linux
2. Pick a starter from the table above
3. Paste the matching skill into Claude / Cursor / Copilot
4. If anything errors, check [`docs/faq/`](docs/faq/) - most beginner errors are listed there
5. Still stuck? Open an issue: https://github.com/axomiyaindie/create-your-first-app/issues

---

## 🛠 Requirements by OS

Every starter needs **Node.js**, **Git**, and a **terminal** (PowerShell / CMD on Windows, Terminal on macOS/Linux). Some stacks need extras:

| Stack | Extra tools |
|---|---|
| Next.js | none beyond Node + Git |
| Astro | none beyond Node + Git |
| Flutter | Flutter SDK, Android Studio (Android), Xcode (iOS, macOS only) |
| Android | Android Studio (Kotlin + Compose), JDK 17 (bundled) |
| Tauri (Windows) | Rust (rustup.rs), Visual Studio C++ Build Tools |
| Tauri (macOS) | Rust, Xcode Command Line Tools |
| Tauri (Linux) | Rust, `libwebkit2gtk-4.1-dev`, `build-essential` |
| Fullstack | none beyond Node + Git (uses SQLite) |

Each starter README lists its own full setup.

---

## 🤝 Contributing

This repo is built to grow. If you can build something, you can add a starter or a skill.

- **Add a starter** - create `starters/<name>/` with a working minimal app + a README
- **Add a skill** - create `skills/build-<stack>-app.md` following the template
- **Fix docs** - any improvement to `docs/` is welcome
- **Fill a placeholder** - iOS, macOS, Linux, or backend (Node/Python/Go/Rust/.NET)

Read [`CONTRIBUTING.md`](CONTRIBUTING.md) for the format each starter and skill must follow.

---

## 📄 License

MIT - see [`LICENSE`](LICENSE).

You can use, modify, sell, and redistribute this repo and everything inside it. Attribution appreciated but not required.

---

## ⭐ If this helped you

Star the repo so others can find it. That is the only "payment" this project asks for.


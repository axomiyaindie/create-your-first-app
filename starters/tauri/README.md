# Tauri Desktop Starter

Lightweight desktop app (Windows / macOS / Linux) using Tauri + a web frontend.

## What is Tauri?
Build desktop apps with web tech (HTML/CSS/JS) and a Rust backend. Much smaller than Electron.

## Prerequisites
- Node.js v18+  ->  `node -v`
- Rust  ->  https://rustup.rs
- Build tools per OS:
  - Windows: Visual Studio C++ Build Tools
  - macOS: Xcode Command Line Tools (`xcode-select --install`)
  - Linux: `sudo apt install libwebkit2gtk-4.1-dev build-essential`

## Create your own copy
```bash
pnpm create tauri-app my-desktop-app
cd my-desktop-app
pnpm install
pnpm tauri dev
```

## Coming soon in this folder
A ready-to-run example app with:
- A Tauri window loading a React frontend
- A native command called from JS
- App icon + build config

## Project structure (once populated)
```
tauri/
  src/               # frontend
  src-tauri/         # Rust backend
    src/main.rs
    tauri.conf.json
  package.json
```

## Next steps
- With AI: use [skills/build-tauri-desktop.md](../../skills/build-tauri-desktop.md)
- Without AI: https://v2.tauri.app/start/


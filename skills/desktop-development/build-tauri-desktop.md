# Skill: Build a Tauri Desktop App

**Goal:** Take a user from zero to a running desktop app (Windows / macOS / Linux) using Tauri + a web frontend.

## Prerequisites check
- `node -v` -> v18+
- `pnpm -v` (or `npm -v`)
- `cargo --version` -> Rust installed (https://rustup.rs)
- Platform build tools:
  - **Windows:** Visual Studio C++ Build Tools
  - **macOS:** `xcode-select --install`
  - **Linux:** `sudo apt install libwebkit2gtk-4.1-dev build-essential`

## Steps

1. **Scaffold**
   ```bash
   pnpm create tauri-app my-desktop-app --template react-ts --manager pnpm
   cd my-desktop-app
   pnpm install
   ```

2. **Ask the user what the app does** (one sentence). Then build:
   - `src/App.tsx` - main UI (window chrome, content)
   - `src/components/` - reusable pieces
   - One native command in `src-tauri/src/main.rs`:
     ```rust
     #[tauri::command]
     fn greet(name: &str) -> String {
         format!("Hello, {}!", name)
     }
     ```
   - Register it in `tauri::Builder::default().invoke_handler(...)`
   - Call it from React with `invoke("greet", { name })`

3. **Run in dev mode**
   ```bash
   pnpm tauri dev
   ```

4. **Build installer**
   ```bash
   pnpm tauri build
   ```
   Output: `src-tauri/target/release/bundle/`

5. **Commit**
   ```bash
   git init && git add . && git commit -m "feat: initial tauri app"
   ```

## Rules for the agent
- Keep the frontend simple (React + Tailwind, no heavy UI kit).
- Native commands go in `src-tauri/src/main.rs` only.
- Never hardcode paths - use Tauri's path APIs.
- Explain each command in one short sentence before running it.

## Done when
- `pnpm tauri dev` opens a native window.
- The `greet` command returns a string from Rust to JS.
- `pnpm tauri build` produces an installer in `bundle/`.


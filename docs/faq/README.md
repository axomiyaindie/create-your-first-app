# FAQ

Common questions and errors from people building their first app.

## General

### Do I need to know how to code?
No. The [skills/](../../skills/) folder contains AI-agent instructions that build apps for you. You describe what you want; the AI writes the code.

### Which stack should I pick?
- **Website / dashboard / SaaS** -> Next.js
- **Blog / docs / landing page** -> Astro
- **Cross-platform mobile** -> Flutter
- **Native Android only** -> Android + Kotlin
- **Desktop app** -> Tauri
- **Full app with login + database** -> Fullstack

### Is this free?
Yes. MIT licensed. All tools have free tiers.

## Install problems

### node is not recognized (Windows)
```powershell
winget install OpenJS.NodeJS.LTS
```
Then close and reopen PowerShell.

### git is not recognized (Windows)
```powershell
winget install Git.Git
```

### pnpm: command not found
```bash
npm install -g pnpm
```
If that fails, just use `npm` instead of `pnpm` everywhere.

## Git problems

### fatal: not a git repository
You are not inside the cloned folder:
```bash
cd create-your-first-app
git status
```

### error: failed to push
```bash
gh auth login
```
Or create a token at https://github.com/settings/tokens.

### LF will be replaced by CRLF
Harmless warning. `.gitattributes` handles it.

### I committed node_modules by accident
```bash
git rm -r --cached node_modules
git commit -m "chore: remove node_modules"
```

## Run problems

### Port 3000 already in use
```bash
npx kill-port 3000
pnpm dev -- -p 3001
```

### Module not found after pulling changes
```bash
rm -rf node_modules pnpm-lock.yaml
pnpm install
```
Windows PowerShell:
```powershell
Remove-Item -Recurse -Force node_modules
Remove-Item pnpm-lock.yaml
pnpm install
```

### Flutter: command not found
Install Flutter: https://docs.flutter.dev/get-started/install

## AI agent problems

### The AI ignores the skill file
Paste the **entire** skill file at the start of the conversation, then say: *"Follow the rules in the above skill strictly."*

### The AI makes up APIs that do not exist
Reply: *"Use mock data first per the skill Rules section."*

### It built something but it does not run
Paste the error back to the AI. It usually fixes itself in one round.

## Contributing

See [CONTRIBUTING.md](../../CONTRIBUTING.md).

## Still stuck?

Open an issue: https://github.com/axomiyaindie/create-your-first-app/issues


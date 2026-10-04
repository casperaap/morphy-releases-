# Morphy — download

**[Download the latest installer](https://github.com/casperaap/morphy-releases-/releases/latest/download/Morphy-Setup.exe)** (Windows)

Morphy is an infinite canvas with AI agents that build little apps ("cards") for you while you talk to them. It runs fully on your computer and uses **your own** AI accounts.

## Installing

1. Download and run the installer. It installs per-user in a few seconds and starts automatically.
2. **Windows will show a blue "Windows protected your PC" warning** — that's because the app isn't code-signed yet (coming later). Click **More info → Run anyway**.
3. Sign in with Google when Morphy opens.
4. Connect your AI accounts in the short setup that follows — or any time later in **Settings → Account** (the gear, bottom left). Then type a message in a chat.

## What you need

At least one of these:

- **Claude** — a Claude subscription. Claude Code comes built in; you only sign in.
- **Codex** — a ChatGPT subscription and the Codex CLI: `npm install -g @openai/codex` (needs [Node.js](https://nodejs.org)).
- **GitHub Copilot** — a Copilot plan and the Copilot CLI: `npm install -g @github/copilot`.
- **Grok** — the Grok CLI (`grok`), signed in with your xAI account.
- **Google Antigravity** — the Antigravity CLI: `winget install Google.AntigravityCLI`, signed in with your Google account.
- **OpenRouter** — connect it in Settings → Account. Free models included. Runs through the Codex CLI, so install that too (see Codex above; no ChatGPT subscription needed).
- **Ollama** — open models on your own computer: [Ollama](https://ollama.com) with a model that can use tools (for example `ollama pull gpt-oss:20b`), plus the Codex CLI.

Updates install themselves automatically — you can switch that off in Settings → General.

## Something broke?

1. Press **Win + R**, paste `%APPDATA%\Morphy\logs` and press **Enter**.
2. Send the **morphy.log** file from that folder to Casper on Discord, together with a screenshot of what went wrong.

Thank you!

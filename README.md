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
- **Grok** — the Grok CLI (`grok`), signed in with your xAI account.
- **OpenRouter** — nothing to install: connect it in Settings → Account. Free models included.

Updates install themselves automatically.

## Something broke?

1. Press **Win + R**, paste `%APPDATA%\Morphy\logs` and press **Enter**.
2. Send the **morphy.log** file from that folder to Casper on Discord, together with a screenshot of what went wrong.

Thank you!

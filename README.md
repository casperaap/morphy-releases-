# Morphy — download

**[Download the latest installer](https://github.com/casperaap/morphy-releases-/releases/latest/download/Morphy-Setup.exe)** (Windows)

Morphy is an infinite canvas with AI agents that build little apps ("cards") for you while you talk to them. It runs fully on your computer and uses **your own** AI accounts.

## Installing

1. Download and run the installer. It installs per-user in a few seconds and starts automatically.
2. **Windows will show a blue "Windows protected your PC" warning** — that's because the app isn't code-signed yet (costs money, coming later). Click **More info → Run anyway**.
3. Sign in with Google when Morphy opens.
4. Type a message in the chat. The first message connects your AI account — a browser/terminal opens, sign in, and your message sends itself.

## What you need

- **Nothing at all** for OpenRouter chats (free models, connects itself in the browser).
- A **Claude** subscription + [Claude Code](https://claude.com/claude-code) installed for Claude chats.
- A **ChatGPT** subscription + Codex (`npm install -g @openai/codex`) for Codex chats.

Updates install themselves automatically.

## Something broke?

Grab the log file at `%APPDATA%\Morphy\logs\morphy.log` and send it to Casper with a screenshot. Thank you!


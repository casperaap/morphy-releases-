# Morphy

**[www.appmorphy.com](https://www.appmorphy.com)** · [Docs](https://www.appmorphy.com/docs) · [Download page](https://get.appmorphy.com)

Morphy is the agentic workspace: all your agents, projects and tools on one canvas. Run Claude Code, Codex, Grok and more side by side, switch projects in a click, and never depend on one AI company. It runs on your own computer and uses **your own** AI accounts.

This repository holds Morphy's installers and release notes. What Morphy does and how to use it is on [appmorphy.com](https://www.appmorphy.com).

## Download

- **Windows:** [Download Morphy-Setup.exe](https://github.com/casperaap/morphy-releases-/releases/latest/download/Morphy-Setup.exe)
- **Mac with an Apple chip (M1 or later):** [Download Morphy-mac-arm64.dmg](https://github.com/casperaap/morphy-releases-/releases/latest/download/Morphy-mac-arm64.dmg)
- **Mac with an Intel chip:** [Download Morphy-mac-x64.dmg](https://github.com/casperaap/morphy-releases-/releases/latest/download/Morphy-mac-x64.dmg)
- **Linux (beta):** see [Morphy on Linux](https://www.appmorphy.com/docs/linux).

Not sure which Mac you have? Apple menu → **About This Mac**: it says **Chip: Apple M…** or **Processor: Intel**. Or just use [get.appmorphy.com](https://get.appmorphy.com), which picks the right download for you.

## Installing

**Windows (10 or 11)**

1. Download and run the installer. It installs per-user in a few seconds and starts automatically.
2. The installer is signed by **Apers**, Morphy's maker. While Morphy is new, Windows may still show a blue **"Windows protected your PC"** screen: click **More info**, check that it says **Publisher: Apers**, then **Run anyway**. If it says **Unknown publisher**, don't run it — that file isn't Morphy.

**Mac (macOS 11 or later)**

1. Open the downloaded `.dmg` and drag **Morphy** into **Applications**.
2. Open Morphy from Applications. The first time, your Mac asks whether you're sure you want to open an app downloaded from the internet: click **Open**. Morphy is signed and checked by Apple.

**Then, on both**

3. Sign in with Google when Morphy opens.
4. Connect your AI accounts in the short setup that follows — or any time later in **Settings → Account** (the gear, bottom left). Then type a message in a chat.

## What you need

At least one of these:

- **Claude** — a Claude subscription. Claude Code comes built in; you only sign in.
- **Codex** — a ChatGPT subscription and the Codex CLI: `npm install -g @openai/codex` (needs [Node.js](https://nodejs.org)).
- **GitHub Copilot** — a Copilot plan and the Copilot CLI: `npm install -g @github/copilot` (or `brew install copilot-cli` on a Mac).
- **Grok** — the Grok CLI (`grok`), signed in with your xAI account.
- **Google Antigravity** — the Antigravity CLI, signed in with your Google account. Windows: `winget install Google.AntigravityCLI`. Mac: `curl -fsSL https://antigravity.google/cli/install.sh | bash`.
- **OpenRouter** — connect it in Settings → Account. Free models included. Runs through the Codex CLI, so install that too (see Codex above; no ChatGPT subscription needed).
- **Ollama** — open models on your own computer: [Ollama](https://ollama.com) with a model that can use tools (for example `ollama pull gpt-oss:20b`), plus the Codex CLI.

Updates install themselves automatically — you can switch that off in Settings → General. Before an update installs, Morphy checks it: on Windows it must be signed by Apers, on a Mac macOS checks Apple's signature.

## Check your download

The Windows and Mac downloads are signed, and every release comes with a **SHA256SUMS.txt** listing the SHA-256 fingerprint of each file (GitHub shows the same fingerprint next to each file).

- **Windows:** right-click the installer → **Properties** → **Digital Signatures**: the signer is **Apers**. Or in PowerShell: `Get-AuthenticodeSignature .\Morphy-Setup.exe` (Status **Valid**) and `Get-FileHash .\Morphy-Setup.exe`.
- **Mac:** signed with the Developer ID **Casper Apers (49CA43438J)** and notarized by Apple. Check with `spctl --assess --type execute -vv /Applications/Morphy.app` (`source=Notarized Developer ID`), and `shasum -a 256` for the fingerprint.
- **Linux:** the AppImage and .deb aren't signed; check them with `sha256sum -c SHA256SUMS.txt --ignore-missing`.

More on how Morphy keeps you safe, and what it doesn't do yet: [appmorphy.com/security](https://www.appmorphy.com/security).

## Security

Found a security problem? Please don't open a public issue: email **security@appmorphy.com**. See [SECURITY.md](SECURITY.md).

## Something broke?

1. Open Morphy's log folder:
   - **Windows:** press **Win + R**, paste `%APPDATA%\Morphy\logs` and press **Enter**.
   - **Mac:** in Finder, choose **Go → Go to Folder…**, paste `~/Library/Application Support/Morphy/logs` and press **Return**.
2. Send the **morphy.log** file from that folder to Casper on Discord, together with a screenshot of what went wrong.

Thank you!

# Security

## Report a problem

Found a security problem in Morphy? Please don't open a public issue. Email **security@appmorphy.com**, or report it privately on GitHub: [Report a vulnerability](https://github.com/casperaap/morphy-releases-/security/advisories/new) (the **Security** tab of this repository). Include:

- what you found, and what someone could do with it,
- the steps to make it happen again,
- your Morphy version (at the top of **Settings → General**) and your system.

We aim to reply within 3 working days, and to fix serious problems as soon as we can. Please give us the chance to fix it before you tell anyone else, 90 days at most. If you like, we'll thank you by name in the release notes of the version that fixes it.

Testing on your own computer and your own account is welcome. Please don't access other people's accounts or data, disrupt Morphy's servers, or try to trick people.

## Supported versions

Only the newest release gets security fixes. Morphy updates itself (unless you turned that off in **Settings → General**), so stay on the latest version.

## What's covered

- The Morphy desktop app for Windows, Mac and Linux, as published in this repository's releases.
- [www.appmorphy.com](https://www.appmorphy.com), [get.appmorphy.com](https://get.appmorphy.com) and api.appmorphy.com.

The AI tools Morphy runs (Claude Code, Codex, Grok, GitHub Copilot, Antigravity, OpenCode and others) belong to the companies that make them. Please report problems in those tools to them.

## Check a download

The Windows installer is signed by **Apers** (Microsoft Artifact Signing). The Mac app is signed with the Developer ID **Casper Apers (49CA43438J)** and notarized by Apple. Every release comes with a `SHA256SUMS.txt`. How to check them: [appmorphy.com/security](https://www.appmorphy.com/security#check).

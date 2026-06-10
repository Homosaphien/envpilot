<div align="center">

# EnvPilot

**The VS Code extension that manages your dev environment — and stops secrets from leaking to GitHub.**

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![VS Code](https://img.shields.io/badge/VS%20Code-1.85+-blue)
![License](https://img.shields.io/badge/license-MIT-green)

</div>

---

> **"I pushed a .env file to a public repo last year. Spent 2 hours rotating credentials."**
> EnvPilot makes that accident structurally impossible.

---

## What it does

### Free — always

| Feature | What it does |
|---|---|
| **Env var viewer** | See all `.env*` files in a clean sidebar panel. Sensitive values are masked by default. |
| **Secret leak detector** | Scans staged files before every commit. Warns you if an API key, password, or private key is about to go public. |
| **Stack detection** | Auto-detects your tech stack from `package.json`, `Dockerfile`, `pyproject.toml`. |
| **Port panel** | Shows all active listening ports and processes — without opening a terminal. |
| **1 saved profile** | Save your current `.env` as a named profile. |

### Pro — $9/mo or $49/yr

| Feature | What it does |
|---|---|
| **Unlimited profiles** | Save as many named environments as you want (dev, staging, production, testing...) |
| **Profile switching** | Switch your entire `.env` with one click in the sidebar. |
| **Onboarding wizard** | Clone a new repo and get a guided setup checklist based on your stack. |
| **Team sync** | Share encrypted `.env` templates with your team. No more Slack DMs with passwords. |

---

## Installation

1. Open VS Code
2. Press `Ctrl+Shift+X` (or `Cmd+Shift+X` on Mac)
3. Search **EnvPilot**
4. Click Install

Or install from the command line:
```bash
code --install-extension PUBLISHER.envpilot
```

---

## Quick start

1. Open any project that has a `.env` file
2. Click the **EnvPilot icon** in the Activity Bar (left sidebar)
3. Your environment variables appear — sensitive values masked
4. Click **Scan staged files** before any git commit to check for leaks

---

## Upgrading to Pro

1. Purchase at [envpilot.dev/pro](https://envpilot.dev/pro) — you get a license key by email instantly
2. In VS Code, open the Command Palette (`Ctrl+Shift+P`)
3. Run **EnvPilot: Activate Pro License**
4. Paste your key — done

---

## Leak patterns detected

EnvPilot scans staged diffs for:

- AWS access keys (`AKIA...`)
- OpenAI / Stripe secret keys (`sk-...`)
- GitHub Personal Access Tokens (`ghp_...`)
- Private key file headers (`-----BEGIN RSA PRIVATE KEY-----`)
- Slack tokens (`xoxb-...`, `xoxp-...`)
- Hardcoded passwords and API keys in any language

---

## Keyboard shortcuts & commands

| Command | Description |
|---|---|
| `EnvPilot: Switch Profile` | Switch active `.env` to a saved profile |
| `EnvPilot: Save Current .env as Profile` | Snapshot current env to a named profile |
| `EnvPilot: Scan Staged Files for Secrets` | Manual leak scan |
| `EnvPilot: Activate Pro License` | Enter your Pro license key |

---

## Privacy

- EnvPilot **never sends your env variables to any server**
- Leak detection runs entirely locally using `git diff --cached`
- License validation sends only your license key to Dodo Payments' API — nothing else
- Pro team sync uses end-to-end encryption before any data leaves your machine

---

## Changelog

### 1.0.0
- Initial release
- Env var viewer with masked sensitive values
- Git pre-commit secret leak detector
- Stack detection (Node, Python, Ruby, Go, Rust, Docker)
- Port & process panel
- Profile save/switch (1 free, unlimited Pro)

---

## Support

- **Issues:** [github.com/YOURUSERNAME/envpilot/issues](https://github.com/YOURUSERNAME/envpilot/issues)
- **Email:** hello@envpilot.dev
- **Twitter:** [@envpilot](https://twitter.com/envpilot)

Built by a developer who got burned. Now you don't have to.

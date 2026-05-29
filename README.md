# Prophet Desktop

> A cross-platform desktop app for **Salesforce B2C Commerce (SFCC)** developers. Watch your local cartridge folders and Prophet Desktop auto-uploads every change to your sandbox the moment you hit save — write code in any editor, keep the server in sync in the background.

A standalone alternative to the **Prophet VS Code extension** and the **JetBrains SFCC plugin** — no editor required.

<img width="1346" height="876" alt="Screenshot 2026-05-29 at 21 43 24" src="https://github.com/user-attachments/assets/89e96832-5fb2-4806-a810-29cc27e7e045" />

This repository hosts the **published releases and the auto-update feed**. To use the app, download an installer from the [Releases](../../releases/latest) page below.

---

## ⬇️ Download

Get the latest version from [**Releases**](../../releases/latest):

| Platform | File |
|----------|------|
| **macOS** (Apple Silicon `arm64` / Intel `x64`) | `.dmg` |
| **Windows** (`x64`) | `.exe` installer |
| **Linux** (`x64`) | `.AppImage` |

Once installed, the app **updates itself automatically** — new versions published here are downloaded in the background, so you stay current without re-downloading.

---

## What it does

**Sync your code, automatically**

- **Connection profiles** — define a profile per SFCC instance (sandbox / dev / staging): hostname, credentials, code version, and the local cartridge folder. Create, edit, duplicate, and delete them; switch the active one with a single click.
- **Auto-upload on save** — a background watcher detects file changes in your selected cartridges and uploads them over WebDAV instantly. Incremental by default — only what changed is sent.
- **Initial / clean sync** — "Upload All" packs every selected cartridge into a zip, uploads it, and unzips on the server for a full clean deploy.
- **Real-time activity** — see exactly what's uploading right now: file, cartridge, target profile, size, progress, and status.
- **Logs** — full operation history with filters by level (info / warn / error), profile, and time, plus expandable request/response detail for debugging failures.
- **Test connection** — validate credentials straight from the profile form before you rely on them.

**Manage the instance, not just the files**

- **Sandbox tools** — a dedicated Sandbox screen with Overview, live **Business Manager logs** streaming, and **Code Versions** management.
- **Code version activation** — list remote code versions and activate one directly from the app via OCAPI.
- **Cartridge path management** — review and reorder a site's cartridge path.

**Stays out of the way**

- **System tray / menu bar** — runs in the background with quick access to pause/resume, Upload All, and profile switching.
- **Native notifications** — alerts on upload failures and key events.
- **Dark & light themes**, English / Ukrainian, keyboard shortcuts, and persisted window state.

## Who it's for

SFCC developers who juggle multiple sandboxes and want one fast, transparent, secure tool to keep code in sync — without wrestling with Ant scripts, `dw.json`, or manual WebDAV uploads.

## Privacy & security

Prophet Desktop is **local-first**. Your credentials are stored in your OS keychain (never in plaintext config), and your code goes straight from your machine to your SFCC instance — there is no cloud middleman, no telemetry, and no account to create.

Built on Electron with hardened defaults: `contextIsolation: true`, `nodeIntegration: false`, `sandbox: true`.

---

## Support

Found a bug or have a feature request? Open an issue on this repository.

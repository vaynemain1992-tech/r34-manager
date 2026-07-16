# R34 Manager

A personal content manager for rule34.xxx — curate franchises and characters, browse and search, download and organize a local library, and clean up duplicates. Runs entirely on your own machine.

**Author:** vaynemain1992 · **License:** Source-available, personal use only (see LICENSE)

---

## Download

**[⬇ Latest installer (Windows 10/11)](../../releases/latest)**

No Python, no Node.js, no command line — just run the installer.

### ⚠️ First-run warning (read this)

The installer is **unsigned**, so Windows SmartScreen will show *"Windows protected your PC"*.
This is expected for independent software:

1. Click **More info**
2. Click **Run anyway**

Some antivirus tools occasionally flag PyInstaller-built apps as a false positive. The SHA-256 hash of each release is listed in its release notes so you can verify your download.

---

## Features

- **Setup wizard** — walks you through connecting your own rule34.xxx account (API key + user ID) with step-by-step instructions, choosing a download folder, and picking starter franchises
- **Curated rosters** — top franchises come pre-loaded with characters instantly
- **Character detection** — three-depth pipeline (quick / standard / deep) that discovers a franchise's characters and picks the correct tag for each
- **Smart downloads** — per-character folder organization, download queue with live progress, "recommended" downloads that grab the top-scored slice of any tag
- **Library** — scan existing folders (with metadata recovery), collections, bulk select, filtering and sorting
- **Visual duplicate finder** — perceptual hashing catches reposts and re-encodes that byte-level comparison misses; one click keeps the best copy of each
- **Backup / restore** — export your whole setup to JSON, import on any machine
- **Diagnostics** — built-in test suite with exportable reports

## Getting your API credentials

1. Create a free account at [rule34.xxx](https://rule34.xxx/index.php?page=account&s=signup)
2. Go to [Account → Options](https://rule34.xxx/index.php?page=account&s=options)
3. Scroll to **API Access Credentials** (click *Generate New Key* if empty)
4. Copy the whole string — the setup wizard splits it into key + user ID automatically

The app works without credentials on the public API, but with lower rate limits.

## Reporting bugs

1. Enable the Debug tab (Settings → Debug mode)
2. Debug → **Run Full Suite** → **Export Report**
3. Send the report file + a short description of what you were doing

## Data & privacy

Everything is local: your database lives in `%LOCALAPPDATA%\R34Manager`, downloads go to the folder you choose, and your API credentials never leave your machine (they're excluded from backups too).

---

© 2025 vaynemain1992. All rights reserved. Personal use only — see [LICENSE](LICENSE).

# Atom

Atom is a free performance app for Windows gaming. It tunes your PC while you play and restores everything when the game closes.

This is the official public repository for Atom:

- **Downloads:** `.msi` installers, release notes and SHA-256 checksums, published under [Releases](https://github.com/DevModee/atom-releases/releases).
- **Issue tracker:** bug reports and feature requests, under [Issues](https://github.com/DevModee/atom-releases/issues).

The application source code is not hosted here.

## Download

**[Download the latest installer (Atom-x64.msi)](https://github.com/DevModee/atom-releases/releases/latest/download/Atom-x64.msi)**

This link always points to the newest release. Past versions and their release notes are on the [Releases page](https://github.com/DevModee/atom-releases/releases).

### Verify the download

Each release includes a [`SHA256SUMS.txt`](https://github.com/DevModee/atom-releases/releases/latest/download/SHA256SUMS.txt) file. In PowerShell, from the folder where you saved the installer:

```powershell
Get-FileHash .\Atom-x64.msi -Algorithm SHA256
```

The hash shown must match the one in `SHA256SUMS.txt`. If it does not, delete the file and download it again.

## Requirements

- Windows 10 version 2004 or later, or Windows 11 (64-bit)
- Administrator rights to install

### Windows SmartScreen

Atom is in open beta and its installer is not signed with an Authenticode certificate yet. Because of that, Windows SmartScreen may warn that the publisher is unknown. If you downloaded the installer from this repository and the hash matches, choose **More info → Run anyway** to continue.

## Report a bug or request a feature

Open an issue at **[github.com/DevModee/atom-releases/issues](https://github.com/DevModee/atom-releases/issues)**. Bug reports are easiest to fix when they include:

- Atom version (shown in **Settings → About**)
- Windows version and build (run `winver`)
- CPU and GPU model
- Steps to reproduce, what you expected and what happened instead
- The diagnostics package from **Settings → Maintenance → Export diagnostics**. Issues are public, so look through it before attaching.

Feature requests are welcome too. Describe what you want to do and why it matters to you.

## Privacy and safety

Atom uses no kernel drivers, no DLL injection and no changes to game memory. Every system change it makes is recorded first and can be reverted.

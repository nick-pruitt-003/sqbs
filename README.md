# SQBS — Sewell's Quiz Bowl Statistics

Tournament scoring and statistics for quiz bowl. This repo is the download home for SQBS now that the original SQBS website is offline.

## Download

All three are on the [SQBS 2.1 release page](https://github.com/nick-pruitt-003/sqbs/releases/latest). Tournament files move freely between them.

| Platform | File | Needs |
|---|---|---|
| **Mac** | [SQBS-2.1-mac.dmg](https://github.com/nick-pruitt-003/sqbs/releases/latest/download/SQBS-2.1-mac.dmg) | macOS 12 or later, Apple Silicon or Intel |
| **Windows** | [SQBS-2.1-win-x64-setup.exe](https://github.com/nick-pruitt-003/sqbs/releases/latest/download/SQBS-2.1-win-x64-setup.exe) | 64-bit Windows |
| **Linux** | [sqbs_2.1_amd64.deb](https://github.com/nick-pruitt-003/sqbs/releases/latest/download/sqbs_2.1_amd64.deb) | 64-bit Debian 12+ or Ubuntu 22.04+ |

What changed in 2.1: [CHANGELOG.md](CHANGELOG.md).

## Opening SQBS on Windows the first time

SQBS isn't signed with a paid certificate. If SmartScreen says **Windows protected your PC**, click **More info**, then **Run anyway**.

## Opening SQBS on a Mac the first time

SQBS is free and isn't signed with a paid Apple Developer ID, so macOS blocks the first launch. You confirm once; after that it opens normally.

1. Open the `.dmg` and drag **SQBS** into **Applications**.
2. In Applications, **right-click** SQBS and choose **Open**, then click **Open** again.
3. **macOS 15 or later:** if there is no Open button, click **Done**, then go to **System Settings → Privacy & Security**, scroll down, click **Open Anyway** next to SQBS, and confirm.

Terminal alternative:

```bash
xattr -dr com.apple.quarantine /Applications/SQBS.app
```

To check the download, compare against the `.sha256` file on the release page:

```bash
shasum -a 256 ~/Downloads/SQBS-2.1-mac.dmg
```

## Source code

| Repo | What it is |
|---|---|
| [sqbs-original](https://github.com/nick-pruitt-003/sqbs-original) | The original Mac SQBS source, archived with permission |
| sqbs-mac (private) | The modernized Mac app these releases are built from |
| SQBSTournamentKit (private) | The shared engine, and the Windows and Linux app |
| [sqbs-plus](https://github.com/nick-pruitt-003/sqbs-plus) | Earlier cross-platform rewrite (Rust + Tauri); its 0.1.0 pre-release stays available |

## Credits

- **Chris Sewell**: original author of SQBS.
- **Neil Smith**, with help from **Ben Smith**: ported SQBS to the Mac.
- **Nick Pruitt**, with assistance from Claude Opus 4.8, 5 and 5.5: Apple Silicon compatibility and modernization.

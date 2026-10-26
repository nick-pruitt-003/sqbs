# SQBS — Sewell's Quiz Bowl Statistics

Tournament scoring and statistics for quiz bowl. This repo is the download home for SQBS now that the original SQBS website is offline.

## Download

| Platform | Get it | Status |
|---|---|---|
| **Mac** (macOS 12+, Apple Silicon and Intel) | [SQBS 2.0.1 for Mac](https://github.com/nick-pruitt-003/sqbs/releases/latest) | Stable |
| **Windows / Linux** | [SQBS Plus](https://github.com/nick-pruitt-003/sqbs-plus/releases) | Pre-release. See the [roadmap](ROADMAP.md) |

What changed in 2.0.1: [CHANGELOG.md](CHANGELOG.md).

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
shasum -a 256 ~/Downloads/SQBS-2.0.1-mac.dmg
```

## Source code

| Repo | What it is |
|---|---|
| [sqbs-original](https://github.com/nick-pruitt-003/sqbs-original) | The original Mac SQBS source, archived with permission |
| sqbs-mac (private) | The modernized Mac app these releases are built from |
| [sqbs-plus](https://github.com/nick-pruitt-003/sqbs-plus) | Cross-platform rewrite (Rust + Tauri) for Windows, Mac and Linux |

## Credits

- **Chris Sewell**: original author of SQBS.
- **Neil Smith**, with help from **Ben Smith**: ported SQBS to the Mac.
- **Nick Pruitt**, with assistance from Claude Opus 4.8, 5 and 5.5: Apple Silicon compatibility and modernization.

# Windows and Linux roadmap

Two efforts exist. Both read and write the same `.qzx`-style tournament files as Mac SQBS and Windows SQBS.

| | SQBS Plus | SQBS (Avalonia) |
|---|---|---|
| Stack | Rust + Tauri + Svelte | C# Avalonia UI on the Swift SQBSTournamentKit engine |
| Repo | [sqbs-plus](https://github.com/nick-pruitt-003/sqbs-plus) (public) | SQBSTournamentKit (private until release) |
| Installers today | v0.1.0 pre-release: Windows `.exe`/`.msi`, Linux `.deb` | None |
| Matches Mac 2.0.1 | Yes, on `main` (merged 2026-08-19), not yet released | Game Entry, Tournament Setup, Reports done; Settings and Merge not started |

## Timeline

**Windows and Linux release: target late October to early November 2026.** Most of the work is done; what remains is finishing and testing Windows compatibility on a PC. Installers will be published in this repo next to the Mac build.

Until then, Windows users can use classic Windows SQBS or the [SQBS Plus 0.1.0 pre-release](https://github.com/nick-pruitt-003/sqbs-plus/releases). Tournament files move between all versions.

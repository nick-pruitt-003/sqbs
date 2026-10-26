# Windows and Linux roadmap

Two efforts exist. Both read and write the same `.qzx`-style tournament files as Mac SQBS and Windows SQBS.

| | SQBS Plus | SQBS (Avalonia) |
|---|---|---|
| Stack | Rust + Tauri + Svelte | C# Avalonia UI on the Swift SQBSTournamentKit engine |
| Repo | [sqbs-plus](https://github.com/nick-pruitt-003/sqbs-plus) (public) | SQBSTournamentKit (private until release) |
| Installers today | v0.1.0 pre-release: Windows `.exe`/`.msi`, Linux `.deb` | None |
| Matches Mac 2.0.1 | Yes, on `main` (merged 2026-08-19), not yet released | Game Entry, Tournament Setup, Reports done; Settings and Merge not started |

## Timeline

<!-- DRAFT: dates below are estimates for Nick to confirm before publishing. -->

1. **SQBS Plus 0.2.0 — target: November 2026.** Release the 2.0.1-parity code already on `main` as Windows and Linux installers. This is the interim PC build.
2. **SQBS (Avalonia) beta — target: Q1 2027.** Remaining work: Settings screens, merge with duplicate detection, then installers that bundle the Swift runtime for Windows and Linux.
3. **SQBS (Avalonia) 2.1 — target: Q2 2027.** Becomes the recommended Windows/Linux download once it has been used at a real tournament. Releases appear in this repo alongside the Mac build.

Until then, Windows users can keep using classic Windows SQBS; files move between all versions.

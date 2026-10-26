# Changelog

## SQBS 2.0.1 for Mac — 2026-10-26

Compared with 2.0 (the May 2026 modernization for Apple Silicon).

### New

- **Manual final-rank override.** Tournament Setup has a Rank column (now the first column). Leave it blank for the computed rank, or type a number to force a team's final rank. The override wins ties. Files with no overrides stay byte-for-byte compatible with Windows SQBS and YellowFruit.
- **Duplicate-game check after a merge.** Merging a playoff file that carries over preliminary games used to double-count them. SQBS now lists games with the same two teams and round and offers **Remove Duplicates** or **Keep All**.
- **Game Entry auto-save.** Leaving Game Entry with a complete, warning-free game records it. Incomplete games, or games that trip an enabled warning, are still discarded. The Record button works as before.
- **W-8: unusual name capitalization** (optional, off by default). Flags likely typos such as `smith`, `SMITH` or `SMith` when a team or player name is entered. It allows particles (de, van), Mc/Mac/O'/D' names, Roman-numeral suffixes (III), and names in scripts without capital letters.

### Fixed

- **Games played as a fraction.** Typing `11/23` in a GP field was read as 11 games. It is now read as 0.478, matching Windows SQBS. Each GP field has a tooltip explaining decimal and fraction entry.
- **Dark Mode.** Tables and text areas no longer show white backgrounds in Dark Mode.
- **Bonus tracking set to None.** After a blocked attempt to change the bonus method, the setting now correctly snaps back to None instead of Manual.
- **Works alongside Quiz Bowl Statkeeper.** Saving a file in SQBS keeps the schedule, pools and playoff data that [Quiz Bowl Statkeeper](https://github.com/bdleblanc81/qbstatkeeper) stores in it.
- **File type.** The app's tournament-file type now matches its declared type exactly, so Finder associates SQBS files correctly.

### Requirements

- macOS 12 Monterey or later (2.0 supported macOS 11). Universal: Apple Silicon and Intel.

## SQBS 2.0 for Mac — 2026-05-11

Modernization of the original SQBS Mac source for current macOS.

- Native Apple Silicon build; macOS 11+.
- Report preview rebuilt on WKWebView (the old WebView was removed from macOS).
- Fixes a crash when merging files with different team counts, wrong Individual Standings sort on one tie-break, Team B standings outside the round range, the "single page" print checkbox being ignored, and several memory leaks.
- Help pages updated for current macOS.

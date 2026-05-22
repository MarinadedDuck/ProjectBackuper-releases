# Project Backuper Releases

Hosts the Sparkle appcast, update ZIPs, and release notes for
[Project Backuper](https://github.com/MarinadedDuck/Project-Backuper) — a
macOS menu-bar app that backs up Adobe project files on a schedule.

## Layout

```
appcast.xml                  # Sparkle feed (served via GitHub Pages)
updates/                     # Signed ZIPs for in-place Sparkle updates
release-notes/               # Per-version HTML, linked from each appcast item
```

## URLs (GitHub Pages)

- Appcast: <https://marinadedduck.github.io/ProjectBackuper-releases/appcast.xml>
- Update ZIPs: `<base>/updates/ProjectBackuper-<version>.zip`
- Release notes: `<base>/release-notes/<version>.html`

## Where new releases come from

Built and signed locally by the
[Project-Backuper repo's release script](https://github.com/MarinadedDuck/Project-Backuper/blob/main/scripts/build-release.sh).
Publishing process is documented in that repo at
[`docs/RELEASE_GUIDE.md`](https://github.com/MarinadedDuck/Project-Backuper/blob/main/docs/RELEASE_GUIDE.md).

**House rule: full ZIP every release, never deltas.** Reasoning is in the
guide.

## Downloads

Direct DMG downloads for first-time installs live on the
[Releases page](https://github.com/MarinadedDuck/ProjectBackuper-releases/releases).
Existing installs receive updates automatically via Sparkle and don't
need to visit this repo at all.

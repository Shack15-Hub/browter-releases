# Browter releases

Signed and notarized builds of Browter for macOS, and the feed the app updates itself from.

This repository holds release assets only. The source is private. Each release carries:

- `Browter-<version>-<arch>.dmg` and its `.sha256`: the download.
- `Browter-<version>-<arch>.zip`: what an installed Browter downloads to update itself.
- `browter-feed-<arch>.json`: the update feed. Browter reads the newest one through `releases/latest/download/`.

Every build is signed as *Developer ID Application: BKey, Inc. (589SHAUPBP)* and notarized by Apple. Releases are published by `scripts/release-local.sh --publish` in the private `brain15-browser` repository.

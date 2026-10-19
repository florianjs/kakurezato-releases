# Kakurezato (隠れ里) — releases

Signed builds of Kakurezato, a private BitTorrent index without a central server or
domain name (Nostr + Tor). This repository only holds release files.

| Platform | File |
| --- | --- |
| macOS (Apple Silicon) | `kakurezato-vX.Y.Z-darwin-arm64.zip` |
| Windows (x64) | `kakurezato-vX.Y.Z-windows-amd64-setup.exe` (per-user, no admin rights) |
| Linux (x64) | `kakurezato-vX.Y.Z-linux-amd64.AppImage` (self-updating) or `.tar.gz` |
| Seedbox daemon | `kakurezato-daemon-vX.Y.Z-linux-{x86_64,aarch64}.tar.gz` (static) |

The app updates itself: it fetches `latest.json` through Tor, checks its signature
against the release key built into the app, and verifies the BLAKE3 hash of the
downloaded file before installing it. Release public key:

```
d5b1422a78d43441a5828a04f30b6e9b95ff3022b9b8e54fbd4228aa1ff24f52
```

`SHA256SUMS` lists the checksums of every file of a release.

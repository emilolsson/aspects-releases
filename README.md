# Aspects — releases

Download the latest build of **Aspects for macOS**:

**[→ Releases](../../releases/latest)**

This repository exists to host the download, and nothing else. The
application's source is private; only the built, signed and notarised
`.dmg` is published here.

Every release carries two files:

| file | what it is |
|---|---|
| `Aspects-<version>.dmg` | the app — signed with a Developer ID and notarised by Apple |
| `Aspects-<version>.dmg.sha256` | its SHA-256, so you can verify the download |

To check a download:

```sh
shasum -a 256 Aspects-<version>.dmg
```

The printed hash should match the contents of the `.sha256` file exactly.

## Why a separate repository

GitHub only serves release assets publicly when the repository itself is
public. Keeping the source private and publishing the binary here is how
the download stays a plain, unauthenticated link — <https://aspectsapp.com>
and the app's own **Check for Updates…** both read this repository's
latest release directly.

## Requirements

macOS 14 (Sonoma) or later, Apple silicon or Intel.

---

Aspects is a deterministic browser motion renderer for macOS.
<https://aspectsapp.com>

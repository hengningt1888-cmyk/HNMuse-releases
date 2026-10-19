# HNMuse releases

Installers, the desktop update feed and the corresponding source for **HNMuse** (恒宁缪斯).
The application's own repository is private; this one holds what a person downloads.

## What is here

| File | Is |
| --- | --- |
| `HNMuse-Desktop-<version>-win-x64.exe` | the Windows installer (NSIS) |
| `latest.yml` | electron-updater's feed: the version, the installer's name, its SHA-512 |
| `HNMuse-Desktop-<version>-win-x64.exe.blockmap` | the bytes the updater fetches a diff from |
| `HNMuse-<version>-source.tar.gz` | the corresponding source of that release (GPL-3.0-or-later) |
| `SHA256SUMS.txt` | SHA-256 of every file above, for a check after downloading |

The desktop app reads the feed from
`https://github.com/hengningt1888-cmyk/HNMuse-releases/releases/latest/download/latest.yml`;
the installer and the block map sit beside it under the same prefix, so the file names in
`latest.yml` are relative and resolve against whichever host serves the release.

## License

HNMuse is free software under GPL-3.0-or-later. Every release carries its corresponding
source as `HNMuse-<version>-source.tar.gz`; that archive is what the licence asks for when
the binaries are handed to someone else. It is built with `git archive` from the commit the
tag points at.

Nothing here is affiliated with Meta or its Muse product.